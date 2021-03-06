### Sources
- https://restfulapi.net/http-status-codes/
- https://en.wikipedia.org/wiki/List_of_HTTP_status_codes
- https://tools.ietf.org/html/rfc2616

### 1xx Informational
- introduced in HTTP/1.1; communicates transfer protocol-level information; the request was received, continuing process
- 100 Continue - headers received, send body
- 101 Switching Protocols - agreeing to switch protocols
- 102 Processing - WebDAV; wait for proper answer; prevents timeout
- 103 Early Hints - returns info in headers before final HTTP response
### 2xx Success
- the request was successfully received, understood, and accepted
- **200 OK** - request was carried out successfully
- **201 Created** - request was carried out and a new resource was created as a result
- 202 Accepted - request has been accepted for processing, but the processing has not been completed
- 203 Non-Authoritative Information - (HTTP/1.1) request was successful but the enclosed payload has been modified from that of the origin server's 200 (OK) response by a transforming proxy (mirror/backup/etc.)
- 204 No Content - server has successfully fulfilled the request and that there is no additional content to send in the response payload body
- 205 Reset Content - server has fulfilled the request and desires that the user agent reset the "document view" which sent the request
- 206 Partial Content - server sent only a part of the response; used when the Range header is sent from the client (ex. to enable resuming a download)
- 207 Multi-Status - WebDAV
- 208 Already Reported - WebDAV
- 226 IM Used
### 3xx Redirection
-  further action needs to be taken in order to complete the request
- 300 Multiple Choices
- 301 Moved Permanently
- 302 Found
- 303 See Other - HTTP/1.1
- 304 Not Modified
- 305 Use Proxy - HTTP/1.1
- 306 Switch Proxy
- 307 Temporary Redirect - HTTP/1.1
- 308 Permanent Redirect
### 4xx Client Error
- the request contains bad syntax or cannot be fulfilled
- **400 Bad Request** - generic request error response; usually request had syntax errors or was too large
- **401 Unquthorized**
- 402 Payment Required
- **403 Forbidden**
- **404 Not Found**
- 405 Method Not Allowed
- 406 Not Acceptable
- 407 Proxy Authentication Required
- **408 Request Timeout**
- 409 Conflict
- 410 Gone
- 411 Length Required
- 412 Precondition Failed
- 413 Payload Too Large
- 414 URI Too Long
- 415 Unsupported Media Type
- 416 Range Not Satisfiable
- 417 Expectation Failed
- 421 Misdirected Request
- **422 Unprocessable entity** - request had semantic errors
- 423 Locked
- 424 Failed Dependency
- 425 Too Early
- 426 Upgrade Required
- 428 - Precondition Required
- 429 Too Many Requests
- 431 Request Header Fields Too Large
- **451 Unavailable for Legal Reasons**
### 5xx Server Error
- the server failed to fulfil an apparently valid request
- **500 Internal Server Error** - generic server error response; uncaught error happened
- 501 Not Implemented
- **502 Bad Gateway**
- **503 Service Unavailable**
- **504 Gateway Timeout**
- 505 HTTP Version Not Supported
- 506 Variant Also Negotiates
- 507 Insufficient Storage
- 508 Loop Deteccted
- 510 Not Extended
- 511 Network Authentication Required