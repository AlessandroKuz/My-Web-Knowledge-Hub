---
tags:
  - URL
  - Uniform-Resource-Locator
  - URI
  - Uniform-Resource-Identifier
  - Protocol
  - Domain
  - Subdomain
  - Port
  - Semantic-URL
---
# URI-And-URL
**URL** stands for **Uniform Resource Locators** and it is a sub-category of **URI** (**Uniform Resource Identifier**).
Each URL points to a single, unique resource. (An exception is when the linked resource does not exist anymore).
A URL is like an #Address, it provides the full information to find a specific place/resource.
## Components
### Protocol/Scheme
Tell the protocol to be used for the request, some examples are:
- #HTTP
- #HTTPS: Which is a secure version of the #HTTP protocol, it is also the default protocol used if none is specified.
- #data
- #mailto
It is usually followed up with `://` or just `:`, for example `http://` or `mailto:`.
### Domain/Authority
Domain name that masks the underlying machines #IP in a human readable address.
The domain is composed in different parts:
- #TLD or #Top-Level-Domain: for example `.com`, .`org` or `.net`
- #Label: is the #Secondary-Level-Domain or #SLD
#### Subdomain
A subdomain is a subsection of the Domain, for example **google.com** is the *domain*, whilst **mail.google.com** is an email-related *subdomain*.
### Port
Optional component.
The domain can also contain a #Port, which indicates the the specific "gate" to be used, when referencing a web resource, it is usually implicit as the #Web-Server already knows that an #HTTP request points to port `80`, while a #HTTPS request point to port `443`, otherwise it is mandatory.
### Path
- Absolute
- Relative: works when referenced within the document
### Parameters
Optional component.
Extra parameters to provide some extra information to the request.
### Anchor
Optional component.
Useful for referencing sections within the same document. It kinda works like a bookmark.
and it is used with an `#`, for example [[URI-And-URL#Anchor]].
## Absolute vs Relative
URLs can be either:
- **Absolute**: when the URL contains all the components needed to locate the resource, for example `https://www.google.com`
- **Relative**: when the missing components get inferred based on the current page.
	- Scheme-relative URL: when only the scheme is missing `//google.com`
	- Domain-relative URL: when the scheme and domain are missing `/index.html`
	- Sub-resource
For relative URL navigation the same logic of a #UNIX path is applied (where `.` indicates the current directory, `..` one directory up and so on...).
## Semantic URLs
Semantic URLs are URLs that abstract away the technical components and only keep the main components, making them easier to use and remember.
For example `google.com/search/puppies` is a #Semantic-URL whereas `google.com/?s=puppies` is not. (EXAMPLE MIGHT NOT WORK BUT ILLUSTRATES THE CONCEPT).