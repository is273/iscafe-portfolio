# Choosing between REST and SOAP API
[Representational State Transfer (REST)](https://en.wikipedia.org/wiki/Representational_state_transfer) 
and [Simple Object Access Protocol (SOAP)](https://en.wikipedia.org/wiki/SOAP) set 
guidelines for APIs which are responsible for data communication across applications. 
Both protocols accomplish the same goal while each provides its own benefits.

## When to use REST
REST, an architectural style, uses standard HTTP to submit a request. Along with using HTTP, the following are some of the benefits REST offers:
- REST supports the use of a range of data formats like HTML, JSON, XML, and plain text.
- REST systems are stateless, using less bandwidth to perform at high levels.
- REST systems are cacheable, allowing websites to collect information temporarily.
- REST can use any protocol, including SOAP.

## When to use SOAP
SOAP, a messaging protocol, allows programs to exchange data with different programs and languages. The following are some reasons to use SOAP:
- SOAP is extendable, allowing Web Service standards to be added.
- SOAP systems can become stateful, storing a client’s information for future requests.
- SOAP features built-in error handling.
- SOAP does not rely on HTTP to handle all requests. SOAP can use Simple Mail Transfer Protocol and Transmission Control Protocol to send messages.

## Which one to use
Both REST and SOAP, while different, are able to accomplish similar results. The following table summarizes the differences between REST and SOAP:
| REST | SOAP |
| ------------- | ------------- |
| Architectural Style | Messaging Protocol |
| Cacheable | Non-Cacheable |
| Stateless | Stateful |
| Supports a range of data formats | Only allows XML |
| Uses HTTP only | Uses HTTP, SMTP, and TCP |
| Can use SOAP | Can’t use REST |
| Basic security | High-level security |
| Efficient and Fast | Secure and Standardized |
