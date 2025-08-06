# APIs: Application Programming Interface
- a set of defined rules and protocols that allows different software applications to communicate with each other
- acts as an intermediary, enabling one application to request services or data from another application without needing to understand the internal workings of that other application
- programmers can use APIs to create software or interact with an external system
- Common examples of APIs include those used for social media integration, payment gateways, weather data, mapping services, and much more
- API is interface(like a barrier) between your Program and and external system

#### Standardized Communication
APIs define how applications should interact, including data formats, request methods, and security protocols.
#### Abstraction
They abstract away the complexity of the underlying system, allowing developers to use functionalities without needing to know the intricate details of their implementation.
#### Interoperability
- APIs enable different applications, even those built with different programming languages or on different platforms, to work together seamlessly.
#### Facilitates Development
- Developers can leverage existing functionalities and data from other services through APIs, accelerating development and reducing the need to build everything from scratch.
the API in action

_______________________________________________________________________________________

## How APIs work
1. Your Application(The Customer)
    - request data or a service(using the rules the API has set)
    - this request is made to the external system
2. The API(The Menu)
    - takes the request and passes it to the external system
    - this API is connected to the external system
    - the external system sets the rules for the API
3. The External System(The Kitchen)
    - processes the request and provides the data or service
    - you must follow the rules of the API to get the data or service
4. API Actions(The Waiter)
    - gets the results from external system and returns the results to you application




#### [Endpoints](./APIs/Endpoint.md)
- a specific, addressable location within an Application Programming Interface (API) where an application can send requests and receive responses

#### [Response Codes](./APIs/ResponseCodes.md)
- messages from the server about the outcome of a page request

#### [Parameters](./APIs/Parameters/README.md)
- allow clients to provide specific instructions or data to influence the API's behavior or the data returned

#### [Headers](./APIs/Parameters/Headers.md)
- contains metadata about the request and the client making it

#### [Authentication](./APIs/Authentication.md)
    - the process of verifying the identity of a client or user, application, or device attempting to access an API
    
#### [Authorization]()
    - process that determines what an authenticated user, application, or device is permitted to do or access within the API
_______________________________________________________________________________________