1. What are the required components of an HTTP request? What are the additional optional components?

The Method (`GET`/`POST`, etc), the Host (DNS/IP address), and the Path are required when making an HTTP request. The Body, Headers, and any Query Parameters are not required.

2. What are the required components of an HTTP response? What are the additional optional components?

The status line will always be included with an HTTP response. The Headers and Body are optional.

3. What determines whether a request should use `GET` or `POST` as its HTTP method?

`GET` should be used when the client is *retrieving* data from a source. `POST` should be used when the client is *adding* or *changin* data in a source.