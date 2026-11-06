# Victory Screen Picker

Tap-to-select map of the lobby TV screens at Victory Church's OKC and Edmond campuses. It runs as a
custom widget inside the Jotform "Digital Signage Request" form: staff tap the screens they want on
a building map instead of ticking a long checkbox list.

- `index.html` is the whole picker. Inside Jotform it reads the widget's `campus` setting (`okc` or
  `edmond`, or `?campus=` in the URL), shows that campus's buildings, and sends the picked screens
  back as the field value, e.g. `E-04 East Vertical, E-13 Coffee Cafe, W-10 Commons`.
- Opened directly in a browser, it runs as a demo with a campus switch.
- `*-base.jpg` are the building maps with the screen badges erased; the page draws the badges.
  Badge positions come from the map source data (`labels.json` / `render_maps.py`) kept with
  Victory's IT notes.
- Screens marked VERT are vertical (tall) screens and need 1080 × 1920 artwork.

No keys, passwords or personal data live in this repo.
