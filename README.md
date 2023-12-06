#### Logout

* Endpoint: /api/auth/logout
* Method: POST
* Request Body:
  * Token (string): User’s access token 

* Response
  * If successful:
    * Status Code: 200
    * JSON Response:
      ```json
      {
        "error": false,
        "message": "Logout Success."
      }

#### Profile
##### Get User Profile

* Endpoint: /api/profile
* Method: POST
* Request Headers:
  * Authorization: Bearer <access_token> 

* Response
  * If successful:
    * Status Code: 200
    * JSON Response:
      ```json
      {
      "error": false,
      "profile":  {
        "email": "ariq123@gmail.com",
        "fullname": "Ariq"
        }
      }

#### Categories
##### Get All Tourist Destination 
* Endpoint: /api/destination
* Method: GET
* Response:
  * Status Code: 200
  * JSON Response:
      ```json
       
           [
            {
            "id": 1,
            "title": "Title 1",
	          "categories" : "Tourist Destination",
            "description" : "Content 1 Description",
	          "Price"	: "20000",
          	"Rate"	: "4.6",
            "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"
            },
            {
            "id": 2,
            "title": "Title 2",
	          "categories":"Tourist Destination",
            "description": "Content 2 Description",
	          "Price"	: "20000",
          	"Rate"	: "4.6",
            "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"
            }
          ]
      
##### Get Tourist Destination by ID
* Endpoint: /api/destination/<destination_id>
* Method: GET
* Response
  * If the content exists:
    * Status Code: 200
    * JSON Response:
        ```json
          {
          "id": 1,
          "title": "Content 1",
	        "categories" : "Tourist Destination",
          "description" : "Content 1 Description",
        	"Price"	: "20000",
	        "Rate"	: "4.6",
          "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"  
          }
  * If content not found:
    * Status Code: 200
    * JSON Response:
        ```json
          {
          "error": "Content Not Found!!"
          }

##### Get All Local Culinary
* Endpoint: /api/culinary
* Method: GET
* Response:
  * Status Code: 200
  * JSON Response:
      ```json
       
           [
            {
            "id": 1,
            "title": "Title 1",
	          "categories":"Local Culinary",
            "description": "Content 1 Description",
	          "Price"	: "20000",
          	"Rate"	: "4.6",
            "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"
            },
            {
            "id": 2,
            "title": "Title 2",
	          "categories":"Local Culinary",
            "description": "Content 2 Description",
	          "Price"	: "20000",
          	"Rate"	: "4.6",
            "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"
            }
          ]
      
##### Get Local Culinary by ID
* Endpoint: /api/culinary/<culinary_id>
* Method: GET
* Response
  * If the content exists:
    * Status Code: 200
    * JSON Response:
        ```json
          {
          "id": 1,
          "title": "Content 1",
	        "categories":"Local Culinary",
          "description": "Content 1 Description",
        	"Price"	: "20000",
	        "Rate"	: "4.6",
          "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"
        }
          
  * If content not found:
    * Status Code: 200
    * JSON Response:
        ```json
          {
          "error": "Content Not Found!!"
          }        

##### Get All Traditional Art
* Endpoint: /api/art
* Method: GET
* Response:
  * Status Code: 200
  * JSON Response:
      ```json
           [
            {
            "id": 1,
            "title": "Title 1",
	          "categories":"Traditional Art",
            "description": "Content 1 Description",
	          "Price"	: "20000",
          	"Rate"	: "4.6",
            "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"
            },
            {
            "id": 2,
            "title": "Title 2",
	          "categories":"Traditional Art",
            "description": "Content 2 Description",
	          "Price"	: "20000",
          	"Rate"	: "4.6",
            "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"
            }
          ]
      
##### Get Traditional Art by ID
* Endpoint: /api/art/<art_id>
* Method: GET
* Response
  * If the content exists:
    * Status Code: 200
    * JSON Response:
        ```json
          {
          "id": 1,
          "title" : "Content 1",
	        "categories" : "Traditional Art",
          "description": "Content 1 Description",
        	"Price"	: "20000",
	        "Rate"	: "4.6",
          "img_url": "https://storage.googleapis.com/bucket_name/image_folder/image_filename.jpg"
        }
          
  * If the content not found:
    * Status Code: 200
    * JSON Response:
        ```json
          {
          "error": "Content Not Found!!"
          }        

### Miscellaneous
#### Homepage
* Endpoint: /index
* Method: GET
* Request Headers:
  * Authorization: Bearer <access_token>
*	Response:
  *	If successful:
    * Status Code: 200
    * Response Body: Hi! Ariq

#### Root
* Endpoint: /
*	Method: GET
*	Response:  
    *	Culturama




      
