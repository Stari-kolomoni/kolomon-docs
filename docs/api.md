# API

## Conventions

### Common Error Codes

Error Code | Description
---------- | -------------
500 | General Backend Exception. Raised whenever a critical action could not be performed.
401 | Authentication Exception. Raised when the user sending the request did not possess sufficient permissions to execute the request.
400 | Invalid Data Exception. Raised when the request data could not be parsed or was otherwise deemed invalid by the server.
404 | Resource Not Found Exception. Raised when the requested data could not be acquired.

### Authentication process
For authentication, JWT tokens are used. Upon login, the client is given an access token with defined expiration time.

When sending requests, client adds in the header of the request the following data:
```
"Authorization": "Bearer <my_access_token>"
```

## Endpoints

TODO