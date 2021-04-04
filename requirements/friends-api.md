# Friends API


## Endpoints


### `GET /v1/friends`

Returns a user's friend list.

RESPONSE
```
{
  "friends": friend[]
}
```

### `POST /v1/friends`

Enables a user's to send friend requests and remove friends from your friend list. 

REQUEST
```
{
  "add": string[],
  "remove": string[]
}
```

### `GET /v1/requests`

Return's a user's pending friend requests.

RESPONSE
```
{
  "requests": request[] 
}
```

### `POST /v1/requests/:id/accept`

Accepts an incoming friend request.

RESPONSE
```
{
  "message": "OK"
}
```

### `POST /v1/requests/:id/decline`

Declines an incoming friend request. 

RESPONSE
```
{
  "message": "OK"
}
```

### `GET /v1/invites`

Returns pending invites for some game. 

REPONSE
```
{
  "invites": invite[]
}
```

### `POST /v1/invites/:id/accept`

Accepts an invation to play a game. 

RESPONSE
```
{
  "message": "OK"
}
```


### `POST /v1/invites/:id/decline`

Declines an invation to play a game. 

RESPONSE
```
{
  "message": "OK"
}
```



