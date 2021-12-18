# provide-postman

## Setup
Clone the project
```
 git clone git@github.com:provideservices/provide-postman.git
```

Open Postman, and select Import <p>

Drag the cloned .JSON files into the Postman drag and drop UI and complete the import


## Environment Configuration

Once imported, create the following three environment variables using your Ident login credentials, leaving the value for `jwt_token` blank:

| Variable | Initial Value     |
| :-------- | :------- | 
| `email` | [insert email] | 
| `password` | [insert password] |
| `jwt_token` | _leave blank_ |


## Authentication

Use the `Authentication` POST request to retreive a `user` `jwt_token`. 

```bash
POST Authentication https://ident.provide.services/api/v1/authenticate
```

The `jwt_token` included in the response will be automatically appended to the environment variable created previously. 

Subsequent requests across all collections will automatically retreive a new token as necessary and save any necessary response data as additional environment variables. 


