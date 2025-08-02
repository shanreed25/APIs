# API Keys
- a unique code provided to an application to authenticate its requests and grant access to an API
- these keys are used to identify which application is making a request, control usage limits, and monitor activity, although they are not as secure as authentication tokens for authorization purposes
- helps prevent unauthorized access to APIs
- identifies the application making an API call, which is useful for debugging and showing usage
- by enabling caching, API keys help minimize API requests and improve application responsiveness
- allows developers to monitor performance, identify bottlenecks, and track application usage
- can be used for load balancing, distributing requests across servers and enhancing scalability

## How API Keys Work
- **Identification**
    -  When an application calls an API, it sends the API key, allowing the API server to identify the calling application.
- **Validation** 
    - The API server verifies the key to check its authenticity and whether it is authorized for the requested resource.
- **Security** 
    - API keys can be sent in various ways, such as in the request header, query string, or as a cookie, but they should be kept secret and are most secure when used with other security measures like HTTPS.
- **Usage Control** 
    - API keys allow for controlling the number of calls to an API and identifying usage patterns and traffic. 