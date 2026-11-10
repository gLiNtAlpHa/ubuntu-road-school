# Ubuntu Road School

An animated, plain-words course for the UK car theory test, in English or Nigerian Pidgin.

- 14 junctions covering the test format and all official DVSA topics
- Moving road scenes, a stopping distance slider, sign flashcards
- The full Highway Code and Know Your Traffic Signs in plain words (21 chapters, 62 signs)
- Three 50-question papers: warm-up, real-test level, and harder than the real test
- Hazard spotting game, random 50-question mock test, and a "fix my mistakes" list

It is one self-contained `index.html`. No build step is needed.

## Host on GitHub Pages

1. Create a new repository and upload these files to the root.
2. Go to **Settings → Pages**, set Source to **Deploy from a branch**, then pick `main` and `/ (root)`.
3. Your site appears at `https://<your-username>.github.io/<repo-name>/`.

Progress is saved in each visitor's own browser (localStorage).

Independent study notes, not from or approved by DVSA. Use the official Highway Code and DVSA practice materials too. Highway Code content summarised from GOV.UK under the Open Government Licence v3.0. Facts checked November 2026.

## Visitor stats

The site sends anonymous stats to GoatCounter. It uses no cookies and collects no personal details.

Stats are already set up with the GoatCounter site code `ubuntu`.
Your dashboard is at https://ubuntu.goatcounter.com.
To turn stats off, delete the two `goatcounter` script tags near the top of `index.html`. To point them somewhere else, change `ubuntu` in the `data-goatcounter` URL and keep the `no_onload` line above it.

What it records:
- Page views: home, each lesson (`/l3`), each Highway Code chapter (`/hc7`), papers (`/set3`), hazard game, mock test.
- Events: `lesson-finished-N`, `chapter-finished-N`, `paper-N-pass-43-50` / `near-35-42` / `mid-25-34` / `low-0-24`, `random-mock-...`, `hazard-game-pass` / `below-pass`, `language-en` / `language-pg`.
- GoatCounter also shows visitors per day, countries, devices and where visitors came from.

The `no_onload` line matters: the course counts its own views (`/l3`, `/hc7`) as you move around, so leaving GoatCounter to also count the page load would double-count the first view.
