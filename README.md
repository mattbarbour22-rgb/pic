# Pick 3 Live — Hub

A single static page with 4 cards linking out to your existing sites:

- Masters → https://the-masters-live.vercel.app/
- PGA Championship → https://pga-championship-live.vercel.app/
- U.S. Open → https://us-open-live.vercel.app/
- The Open → https://the-open-live.vercel.app/

Your 4 original sites are completely untouched — same env vars, same
Supabase state, same admin secrets, same everything. This is just a front
door.

Each card uses the same background photo as that major's own live site
(Masters uses the actual `augusta1.jpg`; the other three use the same
Unsplash photos referenced in their own `tournament.js` files).

## Deploy it (as its own tiny Vercel project)

1. Create a new GitHub repo — for a simpler resulting URL, name it
   something like `pick3comp` (Vercel's default domain follows your
   project name, so `pick3comp` → `pick3comp.vercel.app`, rather than
   something long like `pick3-live-hub`). Push this folder's `index.html`
   and `augusta1.jpg` to it.
2. In Vercel, "Add New Project" → import that repo, and when it asks for
   the project name, use `pick3comp` (or similar). No build settings or
   environment variables needed — it's static files.
3. Optionally point a custom domain at it later.
4. Share that one link. Clicking a card takes people to the right major's
   live leaderboard.

## Updating

If a URL ever changes (e.g. you redeploy a major under a new domain), just
edit the `href` in `index.html` for that card and redeploy.

## If a URL is wrong

I used the addresses you gave me. If any of those aren't the actual live
production URLs (e.g. you're using a custom domain instead of the
`.vercel.app` one), just tell me the correct one and I'll fix the file.
