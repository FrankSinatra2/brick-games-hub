# Pong Game Requirements

## Systems
* Accounts API
* Friends API
* Pong UI
* Pong API


## Accounts System API

Responsible for maintaining who has registered with our software and provides JWTs to be used for authentication.

## Friends System API

Responsible for storing associations between users who have been registered via the Accounts System API. Provide the ability to invite friends to games.

## Pong UI

Allows users to:
  * register
  * send and recieve friend requests
  * invite friends
  * play pong
  * view stats of all players
    - highest rally
    - win / loss 
    - games played

## Pong API

Provides data for on-going game states. Keeps track of players stats