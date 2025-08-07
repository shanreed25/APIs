# Bearer Token
- a digital key or token that grants access to a protected resource, like an API or a web service, to anyone who possesses it
- bearer tokens are a crucial part of both authentication and authorization processes, but more specifically they are a form of authorization, not authentication itself
- initial authentication step (like providing a username/password) is needed to obtain a bearer token
- the token's main function is to grant access to protected resources by proving that the "bearer" of the token is allowed to access the protected resource
- the server verifies the token's validity to grant or deny access

# How Bearer Tokens Work 

1. **Initial Authentication**: A client uses credentials (like a password or OAuth 2.0) to authenticate with an authorization server
2. **Token Issuance**: The server issues a bearer token (a cryptic string) to the client
3. **Authorization in Requests**: For subsequent requests to protected resources, the client includes the bearer token in the Authorization header
4. **Server-Side Validation**: The resource server validates the token (checking its expiry, signature, and permissions) before allowing or denying access to the requested resource


#### Authorization, not just Authentication
**A bearer token acts as a "permit" that proves authorization to access a resource, replacing the need for repeated authentication.**

#### The "Bearer" Concept
**The term "bearer" implies that anyone holding the token can use it to gain access. This makes security critical, especially the use of encrypted protocols like HTTPS.**

#### Common Usage
**Bearer tokens are often used in the OAuth 2.0 framework and in microservices architectures for delegated access and service-to-service communication.**

#### Security Considerations
**Due to the risk of interception, bearer tokens must be transmitted over secure channels (e.g., HTTPS) and stored securely by the client to prevent misuse**



What is Bearer authentication?

Bearer authentication (also known as token authentication) is an HTTP authentication scheme that involves security tokens. The name “Bearer authentication” basically means “give access to the bearer of this token.” The security token or “bearer token” is just a cryptic string. An example of a bearer token would be a string that could look something like this:

"AAAAAAAAAAAAAAAAAAAAAMLheAAAAAAA0%2BuSeid%2BULvsea4JtiGRiSDSJSI%3DEUifiRBkKG5E2XzMDjRfl76ZC9Ub0wnz4XsNiRVBChTYbJcE3F"

The idea is that whoever has the secret token, has permission to interact with the spreadsheet. A client - like your browser or mobile app - would then send this security token in the Authorization header when making requests to Sheety's server.