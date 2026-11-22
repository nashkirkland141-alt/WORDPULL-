WORDPULL MULTIPLAYER BUILD

This build has REAL realtime 1v1 multiplayer using Supabase Realtime Broadcast + Presence.

QUICK SETUP (required once to enable multiplayer):
1. Create a free project at https://supabase.com
2. In Supabase Project Settings > API, copy Project URL and the anon/public key.
3. Open config.js and replace the blank values:
   supabaseUrl: 'https://YOUR-PROJECT.supabase.co'
   supabaseAnonKey: 'YOUR-ANON-PUBLIC-KEY'
4. Deploy the folder to HTTPS hosting (Cloudflare Pages, GitHub Pages, etc.).
5. Open the site from two browsers/devices and press FIND MATCH in each.

No database tables are required for the realtime match itself. The lobby and match use public realtime channels, so use Supabase Realtime and allow public Broadcast/Presence channels in your project's Realtime settings. Do not paste service-role keys into this website.


WHAT IS INCLUDED
- Real player matchmaking (Presence lobby)
- 1v1 realtime match channels
- Shared letter set and match start countdown
- 60 second timer
- Live word pull score updates
- Dictionary validation, tiles, back/clear/shuffle
- Local profile and local rating/stats

LIMITATIONS
- The rating/profile and leaderboard remain browser-local in this build. Global Top 1000, account sign-in, persistent cross-device stats, server-side anti-cheat and production match verification require a database/functions layer. This is not yet a production ranked backend.
- Realtime matchmaking is a simple two-player lobby prototype; it is best for testing and will need server-side matchmaking hardening before public launch.

Files: index.html, style.css, script.js, config.js, assets/
