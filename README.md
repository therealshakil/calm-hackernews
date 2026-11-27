# calm-hackernews

Hacker News in ink and paper.
A calm skin for [news.ycombinator.com](https://news.ycombinator.com), one stylesheet, no script.

Part of the [calm suite](https://github.com/therealshakil/calm).

## What it does

Titles and comments read in Yrsa, a serif.
Scores, ranks and bylines fade back so the words carry the page.
Comments keep a comfortable measure.
It follows your OS into light or dark.

HN stays recognisable.
The bar, the boxed Y, the bold name and the piped nav keep their shape.
The Y keeps a little of its orange, in calm's clay.

## Install (Firefox)

Firefox reads site styles from `userContent.css` in your profile's `chrome` folder.
It only follows an `@import` to a file inside that folder, so put the sheet there.

1. In `about:config`, set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`.
2. Copy or link [`calm-hackernews.css`](./calm-hackernews.css) into `<your-profile>/chrome/`.
3. In `<your-profile>/chrome/userContent.css`, add `@import url("calm-hackernews.css");` above every other rule.
4. Restart Firefox.

Your profile folder is listed in `about:profiles`.
If `userContent.css` is itself a symlink, Firefox won't follow imports from it, so keep it a real file.

## Fonts

Yrsa is embedded in the sheet, because HN's content policy blocks fetched fonts.
Atkinson Hyperlegible and IBM Plex Mono are used by name, so install them for the full look.
Without them it falls back gently to your system faces.

## Notes

Tested in Firefox through `userContent.css`.
It's written for Stylus too (it's wrapped in `@-moz-document`), but that path is untested.
Selectors were checked against HN's markup on 27 Nov 2026; a stale one fails safe and just stops applying.

## Licence

MIT, see [`LICENSE`](./LICENSE).
Yrsa is under the SIL Open Font License, embedded via [Fontsource](https://fontsource.org).
