# StoryVerse

Wattpad-style starter website with accounts, profiles, stories, votes, and a reader.

## Run locally
1. Install Node.js 18+.
2. Run `npm install`.
3. Run `npm start`.
4. Open `http://localhost:3000`.

## Railway deployment
Use a persistent Volume mounted at `/app/data` and set these environment variables:
- `NODE_ENV=production`
- `DB_PATH=/app/data/storyverse.db`
- `SESSION_SECRET` = a long random secret

The app creates the database automatically. Registration/login are required for publishing and voting. Votes start at 0 and each logged-in user can vote once per story (and toggle their vote).
