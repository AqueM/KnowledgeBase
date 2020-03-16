https://restfulapi.net/http-methods/

https://restful-api-design.readthedocs.io/en/latest/methods.html

https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/CONNECT

https://www.w3schools.in/restful-web-services/rest-methods/

###GET
* retrieve resources
* basic responses: 
  * 200 OK when resource found + the resource
  * 400 Bad Request when call was incorrect
  * 404 Not Found when resource not found
 * accepts URL parameters like ?page=1
 * safe (cannot interfere with data)
 * can call either collection or specific resource
 * example uses: pagination, navigation, user details display

#####HEAD
* GET but only requests the Headers
* example use: check before possibly GETting large quantities of data
* safe
  
###POST
* create new resources
* basic responses: 
  * 200 OK when successful but can't return the resource
  * 201 Created when successful + the created resource
  * 204 No Content when successful but can't return the resource (TODO: difference?)
 * not safe (can interfere with data) - definitely needs security measures
 * calls a collection (target folder etc.)
 * try not to use POST for single resource (TODO: why?)
 * example uses: create user or item

###PUT
* update entire resource; swap for new
* basic responses: 
  * 201 Created when resource hadn't previously existed, but was created + the created resource
  * 200 OK when successful (TODO: resource returned?)
  * 204 No Content when successful (TODO: when what?)
  * 400 Bad Request when call is incorrect
  * 404 Not Found when resource missing
  * 405 Method not allowed (when calling entire collection instead of singular item)
 * not safe (can interfere with data) - definitely needs security measures
 * calls a specific resource (by ID etc.)
 * 405 Method not allowed when used on a collection
 * example uses: update user or item 

###DELETE
* remove resource
* basic responses:
  * 200 OK when successful
  * 202 Accepted when action was queued
  * 204 No Content when successful (TODO: when what?)
  * 404 Not Found when resource missing
* not safe (can interfere with data) - definitely needs security measures
* calls a specific resource (by ID etc.)
* 405 Method not allowed when used on a collection
* example use: remove a user or item

###PATCH
* update partial resource (applies a delta diff)
* support not universal (IE8, PHP, Tomcat, DJango... missing support)
* basic responses: 
  * 201 Created when resource hadn't previously existed, but was created + the created resource
  * 200 OK when successful (TODO: resource returned?)
  * 204 No Content when successful (TODO: when what?)
  * 400 Bad Request when call is incorrect
  * 404 Not Found when resource not found
  * 405 Method not allowed (when calling entire collection instead of singular item)
* not safe (can interfere with data) - definitely needs security measures
* calls a specific resource (by ID etc.)
* 405 Method not allowed when used on a collection
* example uses: update user or item 