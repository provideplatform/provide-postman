# provide-postman

## Setup
Clone the project
```
 git clone git@github.com:provideservices/provide-postman.git
```

Open Postman, select `Import`


Drag the cloned .JSON files into the Postman drag and drop UI

Select [Import]




## Environment Confirguration

Once imported, create the following three environment variables using your Ident login credentials, leaving the value for `JWT_token` blank:

| Variable | Initial Value     |
| :-------- | :------- | 
| `email ` | [your email] | 
| `password ` | [your password] |
| `jwt_token ` | _leave blank_ |


`Save` the environment variables and return to the collections


## Authentication

In the Ident collection, send the `Authentication` POST request found in the Tokens folder

```bash
POST Authentication https://ident.provide.services/api/v1/authenticate
```

  
