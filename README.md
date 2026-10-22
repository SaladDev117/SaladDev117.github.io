# SaladDev117.github.io

Root of https://saladdev117.github.io. It exists mainly for files that Android and AdMob only
look for at the root of a domain, which project sites (like `/tagalong-site/`) can't provide.

| File | Purpose | To do |
| --- | --- | --- |
| `.well-known/assetlinks.json` | Android App Links verification for TagAlong invite links (`https://saladdev117.github.io/tagalong-site/join/CODE`), so they open the app directly | After the first upload to Play Console, copy the SHA-256 from *Test and release → App integrity → App signing → App signing key certificate* (or the ready-made "Digital Asset Links JSON" there) and replace the placeholder. Add the upload key's SHA-256 too if you install EAS builds outside Play. |
| `app-ads.txt` | AdMob verification for apps whose Play listing names `https://saladdev117.github.io` as the developer website | Paste the line from AdMob (contains your `pub-…` ID) and uncomment it. |
| `.nojekyll` | Stops Jekyll from dropping the `.well-known` folder | — |
| `index.html` | Small landing page linking each app's policies | — |

Project sites (`/tagalong-site/`, `/handyai-site/`) keep working alongside this one.
