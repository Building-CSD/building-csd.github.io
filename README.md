# Center for Spirituality and Dialogue website

Live site: https://building-csd.github.io/

A single page made with plain HTML and CSS. There's no build step, so whatever you save here is what goes live, usually within a minute or two.

## Editing text

1. On GitHub, open `index.html` and click the pencil icon (Edit).
2. Each section starts with a comment you can search for (Cmd/Ctrl+F):
   `INTRO`, `EVENT BLOCK`, `ABOUT`, `WEEKLY MEDITATION`, `USE THE SPACE`, `GET INVOLVED`, `VISIT`.
3. Change only the words between tags, such as `<p>` ... `</p>`. Leave the angle-bracket parts alone.
4. Click **Commit changes**. The live site updates in about a minute.

## Swapping the featured event

Everything for the event sits between `EVENT BLOCK` and `END EVENT BLOCK` in `index.html`:

- **Title:** the `<h2 id="event-title">` line
- **Date and time:** the `<p class="when">` lines. Also update `datetime="2026-11-15T15:00"` (year-month-dayThour:minute).
- **Description:** the paragraph below the date
- **RSVP link:** the `href="..."` on the "RSVP" button
- **Flier:**
  1. Upload the new image and PDF into the `images` folder (Add file, then Upload files).
  2. Change `images/peace-flier.jpg` and `images/peace-flier.pdf` to the new file names.
  3. Rewrite the `alt="..."` text so it describes the new flier. Screen-reader users hear this text in place of the image.
  4. Keep flier images under about 200 KB. A JPG about 760 px wide works well.

Also update the event text in the `og:description` line near the top. That's the text that shows in link previews on iMessage, Slack and similar apps.

## Optional later

- Photos of the building: there's a spot marked in the About section.
- The flier PDFs in `images/` were rebuilt from images. Upload the original PDFs under the same names to replace them.

## Colors (in `styles.css`)

Sampled from the fliers: green `#175e36`, parchment `#e1c5a5`, ink `#2d2d2d`, brass `#7a5e2a`.
