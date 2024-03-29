---
title: Fetch Games
permalink: /docs/backend/commands/fetchGames
---

# Fetch Games

This command is a non-`auth-required` command used for getting a list of all active games.

Once sent the backend will then process the request and return a list of all the active lobbies.
Those lobbies can have any state. In a upcoming version there might be a filter for states.

NOTE: It does not require any arguments.

## Sample
```json
{
    "command": "fetchgames",
}
```

## Response
```json
{
    "errorCode": 0,
    "message": "OK",
    "jsonData": [
        {
            "gameid": "some-random-uuid-here",
            "players": [
                {}
            ],
            "title": "game-title",
            "maxplayers": 4
        }
    ]
}
```
