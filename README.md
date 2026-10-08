# Louis III's Daily Planner

A lightweight, offline-capable, phone-first daily nap and feeding planner. No backend or account is required for using the app.

## Publish on GitHub Pages

1. Create a new **public** repository, e.g. `louis-daily-planner`.
2. Upload **all** files in this folder to the repository root, including `index.html`, `sw.js`, `manifest.webmanifest`, `icon.png`, `icon-512.png` and `.nojekyll`.
3. Go to repository **Settings → Pages**.
4. Select **Deploy from a branch**, branch **main**, folder **/(root)**, then **Save**.
5. Open `https://YOUR-USERNAME.github.io/louis-daily-planner/` once Pages is published.
6. On the iPhone, open the URL in Safari, tap **Share → Add to Home Screen**, keep **Open as Web App** enabled, then **Add**.

## Storage

All settings and the current day's events are automatically saved in browser localStorage on **that device**. They do **not** sync between phones. Use Export backup before clearing Safari data, deleting the web app, or moving devices. The site itself is publicly accessible; daily schedule data is not uploaded to GitHub.

## Behavior

- Early waking and final wake-up are recorded separately.
- Suggested first nap begins 2h45m after final wake; second begins 3h15m after the first ends; suggested bedtime is 3h30m after nap 2 ends.
- Nap duration defaults to 90 minutes, adjustable 30–120 minutes per nap.
- Four bottles: first 30 minutes after wake, second and third at roughly 4-hour intervals, last 30 minutes before bedtime.
- Two solids meals are coupled to formula 2 and 4, with a configurable lead time.
- Lock or record actual event times; future unlocked suggestions recalculate. Conflicts produce warnings rather than silently overriding a lock.
- New Day clears day-specific entries but keeps preferences. Reset Day clears event adjustments only.

This planner is not a substitute for pediatric advice or feeding cues.
