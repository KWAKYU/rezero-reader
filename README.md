# Re:Zero Reader

A small offline reader for the Re:Zero web novel translations on
[Witch Cult Translations](https://witchculttranslation.com).

The app contains no novel text. Your browser loads chapters from the site's public API
and stores them on that device, so saved chapters open without internet.

## Using it

- **Mac:** double-click `index.html` and it opens in Safari.
- **iPad:** Safari on iPad can't run a local HTML file, so the folder needs a web address
  (e.g. GitHub Pages). Open that address once while online, then
  **Share → Add to Home Screen**. Open it from the Home Screen icon from then on.
  The Home Screen app keeps its own storage, so its saved chapters and reading
  position aren't cleared the way Safari can clear unused website data.

## What it does

- Reopens the chapter you were reading, at the paragraph where you stopped
  (this survives text size and window size changes).
- Chapter list (☰) with arcs and phases, a search box, ✓ for finished chapters and % for
  ones you're partway through. A cloud icon means that chapter isn't saved offline yet.
- **Save offline** downloads a whole arc (Arc 7 is about 3 MB). By default the arc you're
  reading is saved in the background, and the next few chapters are always fetched ahead.
- Display settings (Aa): Auto/Light/Sepia/Dark theme, serif/sans font, text size,
  line spacing and page width.
- Mac keyboard: ← / → for the previous/next chapter, Esc closes panels.
- Checks the site for new chapters every few hours while you're online.

Reading position is stored separately on each device.

## Files

- `index.html`: the whole app
- `sw.js`, `manifest.webmanifest`, `icons/`: let it install and open offline when it's served from a web address
