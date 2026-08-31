ROCK LOBSTERS LINEUP BUILDER  —  Hosted version
================================================

WHAT'S IN HERE
  index.html        The app (reads cards from the /cards folder).
  cards.json        The roster list — one line per player card filename.
  cards/            All player card PNGs (number_lastname.png).
  backgrounds/      The 3 page backgrounds.

Upload ALL of these (keep the folder structure) to your GitHub repo,
then Netlify publishes them. Hand the broadcaster your Netlify link.

IMPORTANT: this version must be opened from a web address (your Netlify
link). Double-clicking index.html on your computer will NOT work — it
needs to be served, which is exactly what Netlify does.

------------------------------------------------
PUSHING UPDATES
------------------------------------------------
ADD or REPLACE A PLAYER CARD
  1. Put the PNG in the cards/ folder (name it number_lastname.png,
     e.g. 12_BANDURKIN.png). If you're replacing an existing card,
     give it a slightly new filename (bump the version, e.g. _v2)
     so browsers grab the new one instantly.
  2. Add (or update) that filename's line in cards.json.
  3. Commit. Live in ~30 seconds. No app rebuild needed.

UPDATE THE APP ITSELF (new feature from Claude)
  1. Replace index.html with the new one.
  2. Commit. Live in ~30 seconds. The broadcaster's bookmark updates
     automatically.

cards.json is just a list, like:
[
  "12_BANDURKIN.png",
  "74_MACK.png"
]
Add a line when you add a card; remove a line to hide one.
