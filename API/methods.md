https://restfulapi.net/http-methods/

###GET
* retrieve resources
* basic responses: 
  * 200 OK when resource found + the resource
  * 400 Bad Request when call was incorrect
  * 404 Not Found when resource not found
 * accepts URL parameters like ?page=1
 * safe (cannot interfere with data)
 * can call either collection or specific resource
 * example uses: pagination, navigation
  
###POST
* create new resources
* basic responses: 
  * 200 OK when successful but can't return the resource
  * 201 Created when successful + the created resource
  * 204 No Content when successful but can't return the resource (TODO: difference?)
 * not safe (can interfere with data)
 * calls a collection (target folder etc.)
 * example uses: create user or item

###PUT
* update entire resource; swap for new
* basic responses: 
  * 201 Created when resource hadn't previously existed, but was created + the created resource
  * 200 OK when successful (TODO: resource returned?)
  * 204 No Content when successful (TODO: when what?)
  * 400 Bad Request when call is incorrect
  * 404 Not Found when resource not found
  * 405 Method not allowed (when calling entire collection instead of singular item)
 * not safe? (can interfere with data)
 * calls a specific resource (by ID etc.)

###PATCH
* update partial resource (applies a delta diff)
* support not universal (IE8, PHP, Tomcat, DJango... missing support)


###DELETE