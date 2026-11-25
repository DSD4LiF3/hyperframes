# REVIEW: HyperFrames promo (A + C mix)

## Creative calls

- Built storyline A ("The file is the film") for 0–18 s and C's payoff ("Same input, same frames") for 18–24 s, ending on A's end card. B ("Change one word") was not built because it needs desktop app screenshots that can't be captured here.
- Everything that claims to be the product is real:
  - The code in the editor is the actual source of `compositions/title.html`, so the title scene is literally the file shown.
  - The terminal lines copy the format of a real `hyperframes render` run in this repo.
  - The mark is the repo's own `docs/logo/light.svg`, split into its two symbol halves and the wordmark.
- The render's frame counter and percentages are illustrative values in the real CLI's own stage format. No render time is shown, because none was measured for this film.
- The edit on screen (#3CE6AC → #06E3FA) is shown as a demo. The file on disk keeps the mint value so the opening stays mint.

## Measured vs looked at

- `lint`: 0 errors, 0 warnings. `check`: ok.
- Seams at 3, 11, 18 and 24 s were checked on strips from −0.2 s to +0.2 s. The title → player cut is frame-identical, and render → filmstrip lands the shrunk player on the centre cell.
- Phone sheet at 360 px: titles and the end card read; the code and terminal are texture at that width, which is accepted.
- Nobody heard it, because there is no sound.

## Warnings kept on purpose

- `film_silent`: there's no music source (no HeyGen sign-in). Add a bed as an `<audio id="music">` in `index.html`, with clicks on the cursor click at 7.75 s and key ticks during typing (8.0–8.4 s, 12.0–13.05 s, 26.9–27.85 s).
- `line_unread` on the code pane: the code is evidence, not copy to read line by line. The one line that matters, the hex value, is highlighted and retyped.
- `contrast_aa_failure` at 15 s: this is editor text that the terminal covers on purpose.

## Weakest shot / next

- The payoff (≈21.4 s), where the two strips converge, is quiet: identical strips merging reads as "one strip", not "two renders matched". With more time, add a beat where B is offset by half a frame and visibly snaps into alignment, and give it a riser and impact once there is sound.
- The title holds about 2 s after line 2 lands (1.1–3.3 s). That's fine for reading, but it could open the pull-back 0.5 s earlier.
