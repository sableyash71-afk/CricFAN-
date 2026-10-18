# CricFAN cricket score app

## Files
- `index.html` — app layout
- `styles.css` — dark navy, pink and peacock-green responsive design
- `index.js` — match list, search, pinning, manual scoring, scorecards, calculations and API polling adapter

## Run
Open `index.html` in a browser or serve this folder with a static web server. The UI is mobile-responsive and suitable as the front end for an Android WebView/PWA wrapper.

## Important score-data note
The included match scores and fixtures are **illustrative demo data**, not verified current international scores. Google Search does not provide a general public live-cricket-score API for unrestricted use. To display real scores, choose a licensed score-data provider, set `API_BASE` in `index.js`, and adapt `fetchLiveScores()` to its response schema. Do not put a private API key in public client-side JavaScript; proxy it through a backend. The code polls the configured endpoint every 1 second, but provider updates and rate limits may be slower. It does not fabricate new real-world scores every second.

## Manual scoring
Open a card's Full scorecard. Run buttons, wides, no-balls, byes, leg-byes, wickets, new batters/bowlers and Undo are included. Runs, balls, boundaries, overs, run rate, and basic bowling figures are calculated in the browser.
