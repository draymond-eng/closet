# The Washington Closet 🚪👔👗

A his-and-hers closet app for designing, organizing, and getting dressed — together.

## Three tabs

- **🛠 Design** — drag pieces (hanging rods, shelves, drawers, shoe shelves, cubbies,
  a hamper) into closet sections, claim sections for each person, and get a to-scale
  drawing, a hanging-space fairness verdict, a shopping list, saved designs, and a
  printable spec sheet.
- **📷 Wardrobe** — snap photos of your closet, then let Claude catalog every item it
  sees (name, color, category, whose it likely is). Add items by hand too. Then ask
  Claude for an organizing plan that matches your wardrobe to your closet design,
  section by section.
- **✨ Outfits** — tell it the occasion, weather, and who's getting dressed, and Claude
  picks 2–3 outfit options using only the clothes you actually own.

## Setup

It's one self-contained `index.html` — open it in a browser, or enable GitHub Pages
on this repo and visit the published URL.

The Wardrobe and Outfits features call the Claude API directly from your browser
(model: Claude Opus 5, via the official `@anthropic-ai/sdk`). Click **⚙︎ Claude** and
paste an Anthropic API key from [platform.claude.com](https://platform.claude.com).
The key, your photos, and your item catalog are all stored only in your browser
(localStorage + IndexedDB) — photos are sent to Claude only when you press "Analyze."
