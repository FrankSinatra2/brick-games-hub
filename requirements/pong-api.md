# Pong API


## Endpoints

### `GET /v1/games`

Returns the list of active games.

RESPONSE
```
{
  "games": game[]
}
```

### `POST /v1/games/:id/join`

Joins a fresh game. Marks game with id :id as in progress. Cannot join an in-progress game.

REQUEST
```
{
  "player": player
}
```

RESPONSE
```
{
  "game": game
}
```

### `POST /v1/games/:id/kick`

Removes a player from the current game.

REQUEST
```
{
  "player": player
}
```

RESPONSE
```
{
  "message": "OK"
}
```

### `POST /v1/join`

Lets a user join the pong server

RESPONSE
```
{
  "player": player
}
```

### `GET /v1/players`

Returns a list of all players who have joined the pong server. 

RESPONSE
```
{
  "player": player[]
}
```


### `GET /v1/players/:id`

Returns the stats for a given player.

RESPONSE
```
{
  "player": player
}
```
