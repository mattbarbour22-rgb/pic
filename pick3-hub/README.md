# Pick 3 Live — Hub

A single static page with 4 cards linking out to your existing sites:

- Masters → https://the-masters-live.vercel.app/
- PGA Championship → https://pga-championship-live.vercel.app/
- U.S. Open → https://us-open-live.vercel.app/
- The Open → https://the-open-live.vercel.app/

Your 4 original sites are completely untouched — same env vars, same
Supabase state, same admin secrets, same everything. This is just a front
door.

## Deploy it (as its own tiny Vercel project)

1. Create a new GitHub repo (e.g. `pick3-live-hub`) and push this folder's
   `index.html` to it.
2. In Vercel, "Add New Project" → import that repo. No build settings or
   environment variables needed — it's a static file.
3. Give it a clean domain (e.g. `pick3.yourdomain.com` or just use the
   `.vercel.app` one Vercel assigns).
4. Share that one link. Clicking a card takes people to the right major's
   live leaderboard.

## Updating

If a URL ever changes (e.g. you redeploy a major under a new domain), just
edit the `href` in `index.html` for that card and redeploy.

## If a URL is wrong

I used the addresses you gave me. If any of those aren't the actual live
production URLs (e.g. you're using a custom domain instead of the
`.vercel.app` one), just tell me the correct one and I'll fix the file.
