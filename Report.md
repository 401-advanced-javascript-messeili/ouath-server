# OAuth Comparative Analysis

## OAuth Provider Name: LinkedIn

### Research Conducted By

- Osama Althabteh
- Mohammad AlEsseili
- Dina Alsaid

### Overall Score and Comments

#### Score (Out of 10): 9

#### General Comments

A back-end application, with in-memory database.
Uses a middleware to Authorize user access to third-party provider.
Login authorization using LinkedIn as an OAuth provider.

#### Pros

- Login using LinkedIn account
- No need for saving user passwords in database
- Easy to integrate in the server

#### Cons

- You need to create an organization in LinkedIn to be able to use the OAuth provider API
- One token every 30 minutes
- limited to 500 requests per day

### Ratings and Reviews

#### Documentation

A back-end application, Utilizing express server, with an in-memory database. Where the front-end is used to show the retrieved data in JSON format.
Uses a middleware to Authorize user access to third-party provider, giving them access to public information to the user's linkeIn account.
Login authorization using LinkedIn as an OAuth provider.
The app is deployed to Heroku.

#### Systems Requirements

Above and beyond 'node' and 'linux', what dependencies or core requirements exist for this framework? Can it play at AWS/Heroku? Does it require a certain database?
Dependencies:

- "base-64": "^0.1.0"
- "bcrypt": "^3.0.7"
- "cors": "^2.8.5"
- "debug": "^4.1.1"
- "dotenv": "^8.2.0"
- "express": "^4.17.1"
- "jsonwebtoken": "^8.5.1"
- "morgan": "^1.9.1"
- "superagent": "^5.1.3"

#### Ramp-Up Projections

How long would/should it take a team of mid-junior developers to become productive? 3-4 hours

### Links and Resources

- [docs](https://docs.microsoft.com/en-us/linkedin/shared/authentication/client-credentials-flow)
- [tutorial](https://www.youtube.com/watch?v=jYflkIo1R4A)

### Code Demos

- [live/running application](https://oauth-server-messeili.herokuapp.com/)
- [code repository](https://github.com/401-advanced-javascript-messeili/ouath-server)

### Operating Instructions

- `npm start`
- `nodemon`
- Endpoint: `/`
  - main page with login button
- Endpoint: `/oauth`
  - Returns a JSON object with the generated token and the username.
