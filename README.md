# Chesster

**Chess**ter is an API/Service that provices Chess playing capabilities.  It is my intention to provide user management, single player, multiplayer, and chat capabilities.

## API

Below is the preliminary API.  [Swagger](http://swagger.io) docs will follow.

| Action | Path | Description |
|--------|------|-------------|
| POST      | /users/    | Creates a new user account |
| GET       | /users/    | Searches for users (query params needed) |
| GET       | /users/:id | Returns information for a user |
| PUT/PATCH | /users/:id | Updates a user account |
| DELETE    | /users/:id | Deletes a user account |
| GET       | /users/:id/matches | Returns information about matches played |
| POST      | /match/    | Creates a new chess game |
| GET       | /match/:id | Returns the current state for a game |
| PUT/PATCH | /match/:id | Updates the game state (makes a move) |
| WS        | /chat      | WebSocket channel for chat |

## Getting Started

### Dependencies

Postgresql 9.3+

### Running
To start your Phoenix app:

  1. Install dependencies with `mix deps.get`
  2. Create and migrate your database with `mix ecto.create && mix ecto.migrate`
  3. Start Phoenix endpoint with `mix phoenix.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](http://www.phoenixframework.org/docs/deployment).

## Learn more

  * Official website: http://www.phoenixframework.org/
  * Guides: http://phoenixframework.org/docs/overview
  * Docs: http://hexdocs.pm/phoenix
  * Mailing list: http://groups.google.com/group/phoenix-talk
  * Source: https://github.com/phoenixframework/phoenix
