# Accounts API


## Endpoints

### `POST /v1/authenticate`

provides a JWT for valid account information.

REQUEST 
```
{
  "username": string,
  "password": string
}
```

RESPONSE
```
{
  "access_token": JWT
}
```


### `POST /v1/accounts/create`

Creates an account for a new user.

REQUEST
```
{
  "username": string,
  "password": string
}
```

REPONSE
```
{
  "username": string,
  "password": string,
  "id": string
}
```

### `GET /v1/accounts/:id`

Returns the details of an account.

RESPONSE
```
{
  "username": string,
  "password": string,
  "permissions": permission[]
}
```

### `POST /v1/accounts/:id/permissions`

Allows APIs to modify the permissions of an account.

REQUEST
```
{
  "add": permission[],
  "remove": permission[]
}
```

### `GET /v1/accounts/:id/permissions`

Returns the detailed permissions of an account.

RESPONSE
```
{
  "permissions": permission[]
}
```