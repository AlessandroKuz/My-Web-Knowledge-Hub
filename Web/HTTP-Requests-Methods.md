---
tags:
  - HTTP
  - HTTP-Requests-Methods
  - safe
  - idempotent
  - cacheable
links:
  - https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods
---
# HTTP-Requests-Methods
## Proprieties
- #safe
- #idempotent
- #cacheable
## Methods
- #GET
- #HEAD
- #POST
- #PUT
- #DELETE
- #CONNECT
- #OPTIONS
- #TRACE
- #PATCH 

| Method                                                                                   | Safe | Idempotent | Cacheable    |
| ---------------------------------------------------------------------------------------- | ---- | ---------- | ------------ |
| [`GET`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/GET)         | Yes  | Yes        | Yes          |
| [`HEAD`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/HEAD)       | Yes  | Yes        | Yes          |
| [`OPTIONS`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/OPTIONS) | Yes  | Yes        | No           |
| [`TRACE`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/TRACE)     | Yes  | Yes        | No           |
| [`PUT`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/PUT)         | No   | Yes        | No           |
| [`DELETE`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/DELETE)   | No   | Yes        | No           |
| [`POST`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/POST)       | No   | No         | Conditional* |
| [`PATCH`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/PATCH)     | No   | No         | Conditional* |
| [`CONNECT`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/CONNECT) | No   | No         | No           |
* #POST and #PATCH are #cacheable when responses explicitly include freshness information and a matching [Content-Location](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Content-Location) header.