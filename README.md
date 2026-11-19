# SoundPrint

Standalone browser-based analytics prototype. Open `index.html` in a browser; no installation required. The demo uses simulated listening events and mood labels, not live Spotify data. To publish, push this folder to a GitHub repository and configure Settings > Pages > Deploy from a branch > main > /(root).

## Build toward Spotify integration
1. Register an app in the Spotify Developer Dashboard and configure an exact redirect URI.
2. Implement Authorization Code with PKCE; never put a client secret in browser code.
3. Verify available scopes and endpoints in the current Spotify documentation: https://developer.spotify.com/documentation/web-api
4. Normalize accessible recently played/top-items responses into the dashboard record shape. Full history requires an account data export or ongoing collection.
5. Replace simulated records in demo.js; keep illustrative moods separate from verified data.
6. Validate filters, aggregations, comparisons and insight exports; handle rate limits, authorization expiry and missing fields.

Files: index.html, demo.js, style.css. The current demo is a front-end starter, not an authenticated Spotify client.
