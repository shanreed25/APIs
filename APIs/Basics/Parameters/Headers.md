# Request Header
- request header is a part of an HTTP request
- contains metadata about the request and the client making it
- headers provide crucial context to the server, allowing it to tailor its response to the client's specific needs
- are formatted as case-insensitive key-value pairs
    - `Cookie: "my_cookie"`
- **Client to Server**: Request headers are sent by the client (like a web browser) to the server
- **Server-side processing**: The server uses this information to understand and fulfill the request


#### Request Headers Examples
- **Accept**: Indicates the media types (like JSON or HTML) that the client can understand.
- **User-Agent**: Identifies the client software, such as the browser and its version.
- **Authorization**: Carries credentials for accessing restricted resources.
- **Cookie**: Contains data previously stored by the server on the client for personalization or tracking.
- **Cache-Control**: Provides instructions to the server about how to cache the response

# Why Request Headers

- in the below python code the token and username are being sent as parameters with the get request
- this is what it would look like in the browser
    - `"https://mywebsite.org/mypictures?token="thisismytoken"&username="myusername"`
```
user_params = {
    "token": "thisismytoken", 
    "username": "myusername", 

}
res = rq.post(url="https://mywebsite.org", json=user_params)
```
- sending parameters this way can exspose our secret stuff(token, username etc...) to bad actors who are looking to steal your secret stuff
- **`https`**: Hypertext Transfer Protocol Secure, prevents data interception by encrypting information, verifies the website's identity through digital certificates, and provides integrity, ensuring data isn't tampered with during transmission
- even though the url is using `https` there are certain cases where this might leak you secret stuff to somebody that you dont want to have it
    - like if someone has installed something that is monitoring your browser
- so some api providers want you to provide the authentication in the header
