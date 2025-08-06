# API authentication
- the process of verifying the identity of a client or user, application, or device attempting to access an Application Programming Interface (API)
- answers the question, "Who are you?", and  establishes who you are
- ensures that the entity making the request is legitimate and not an imposter
- ensure that only authorized entities can interact with the API and access its resources, by ensuring that the entity making the request is legitimate and not an imposter

## API Authentication Process 
#### Credential Submission:
- when a client wants to access an API, it sends a request that includes some form of authentication credentials. The specific type of credentials used depends on the authentication method implemented by the API (e.g., API keys, tokens, username/password).
#### Credential Validation:
- the API receives the request and validates the provided credentials against its stored information or by interacting with an identity provider.
#### Access Grant or Denial:
- if the credentials are valid and the client is authorized, the API grants access to the requested resources. Otherwise, the request is denied, often with an authentication error.
_________________________________________________________________________

## API authentication Methods
**Various methods exist, and each has its own characteristics and suitability for different use cases.**
#### API Keys:
- simple token-based access, often used for internal services or when a high level of security isn't the primary concern.
#### OAuth 2.0:
- an authorization framework widely used for third-party integrations, allowing access without sharing user credentials directly with the client application.
#### JSON Web Tokens (JWT):
- self-contained, stateless tokens that can be used for authentication in microservices architectures.
#### Basic Authentication:
- sends username and password in the request headers, typically used in legacy systems.
#### Bearer Token Authentication:
- token-based access via the Authorization header, common in modern web APIs.
#### Mutual TLS (mTLS):
- uses certificates for mutual verification between client and server, providing a high level of security for sensitive systems.