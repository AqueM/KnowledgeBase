####Sources
- https://restfulapi.net/soap-vs-rest-apis/
- https://blog.i-systems.pl/soap-vs-rest/

###SOAP
- Simple Object Access Protocol
- a new protocol (over HTTP) for developing SOAP-based APIs
- can use XML only
- when binding to HTTP, all SOAP requests are sent through HTTP POST
- when not binding to HTTP, independent of platform, language and transport method
- security is well standardized through WS-SECURITY
- more complex and thus more difficult to develop
- standardized, also has built-in error handling
- used in high-risk and highly-standardized projects (ex. finances)

###REST
- REpresentational State Transfer 
- an architectural style (no new technology or standard; almost synonymous to HTTP)
- can use any machine-readable format, like JSON (most commonly), CSV, YAML, RSS
- uses HTTP methods: GET, POST, PUT, DELETE, PATCH
- HTTP is an unsecure protocol needs additional implementation on server level
- simpler, more limited
- easier to learn
- faster, more efficient
- widely used in most web applicaitons