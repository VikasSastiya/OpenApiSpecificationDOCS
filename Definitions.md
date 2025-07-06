## Definitions

## 3.1 OpenAPI Document
A self-contained or composite resource which defines or describes an API or elements of an API. The OpenAPI document MUST contain at least one paths field, a components field or a webhooks field. An OpenAPI document uses and conforms to the OpenAPI Specification.

## 3.2 Path Templating
Path templating refers to the usage of template expressions, delimited by curly braces ({}), to mark a section of a URL path as replaceable using path parameters.

Each template expression in the path MUST correspond to a path parameter that is included in the Path Item itself and/or in each of the Path Item’s Operations. An exception is if the path item is empty, for example due to ACL constraints, matching path parameters are not required.

The value for these path parameters MUST NOT contain any unescaped “generic syntax” characters described by [RFC3986] Section 3: forward slashes (/), question marks (?), or hashes (#).

## 3.3 Media Types
Media type definitions are spread across several resources. The media type definitions SHOULD be in compliance with [RFC6838].

Some examples of possible media type definitions:

  text/plain; charset=utf-8
  application/json
  application/vnd.github+json
  application/vnd.github.v3+json
  application/vnd.github.v3.raw+json
  application/vnd.github.v3.text+json
  application/vnd.github.v3.html+json
  application/vnd.github.v3.full+json
  application/vnd.github.v3.diff
  application/vnd.github.v3.patch
## 3.4 HTTP Status Codes
The HTTP Status Codes are used to indicate the status of the executed operation. The available status codes are defined by [RFC7231] Section 6 and registered status codes are listed in the IANA Status Code Registry.
