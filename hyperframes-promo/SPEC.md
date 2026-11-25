# SPEC: HyperFrames promo, "The file is the film" (A + C mix)

GOAL: the viewer leaves thinking "my video is just a web page I can edit, and it renders the same every time", then types the install command.
OUTPUT: HyperFrames, 1920 x 1080, 30 fps
TIME: 30 s x 30 = 900 frames. Silent: no music source (no HeyGen sign-in); type and picture carry it.

LOOK:

- Worlds: (1) the video: mint #3CE6AC ground, ink #181716; after the edit, cyan #06E3FA ground. (2) the workspace: the docs' own ground #f2f0ed, white panes #ffffff, 1 px #e3e0db border, radius 18, shadow 0 24 60 rgba(24,23,22,0.12). (3) the terminal: #181716 pane, text #f2f0ed, prompt and progress in mint #3CE6AC.
- Type: Inter 900, -4.5% tracking. Hero title 230 px; headlines 96 px; tagline 48 px. Code and terminal: JetBrains Mono 26-28 px, line height 46 px.
- Accent: the logo gradient #06E3FA -> #4FDB5E, only on the mark; mint only as the video's ground, the terminal prompt and the marker behind "frames.".
- No grain, no vignette, no glow.

OBJECTS:

- The player: the real video frame (a live copy of the title scene) with a play bar under it: 6 px track, ink playhead.
- The editor: a code pane with a file tab "compositions/title.html", line numbers in #a8a29e and code in ink. The hex value is selected with a mint highlight, then retyped.
- The terminal: real `hyperframes render` output lines (taken from an actual render in this repo), with a 25-cell block progress bar and a "Streaming frame n/900" counter.
- The filmstrip: #181716 band with #f2f0ed sprocket holes 18x12 every 48 px, 384x216 cells showing the title film's frames.
- The mark: the repo's own logo files (docs/logo/light.svg), split into its two symbol halves and the wordmark.

MOTION:

- Arrivals: expo.out / power4.out. Camera pull-backs: power2.inOut, 0.8 s. Exits: power3.in, about 0.5 s.
- Titles: per-line blur 8 -> 0 in 0.2 s, or per word blur in 0.13 s, 0.07 s apart. Once landed, they hold dead still.
- Typing: stepped clip reveal, 1 step per character, about 0.06 s a character.

SHOTS:

1. 0.0-3.0 title: mint full frame. "Write HTML." is already resolving at frame 0, and "Render video." blurs in at 0.9. Hard match into 2.
2. 3.0-11.0 editor: the identical frame pulls back into a player (0.3-1.1), which scrubs back and forth (1.2-2.4). It pulls back again (2.5-3.3) as the editor slides in from the left and "It's just HTML." lands. The cursor enters from off-screen, clicks the hex value and retypes #06E3FA, and the player floods cyan at about 5.7. The cursor leaves downward, and the editor becomes the terminal in 3.
3. 11.0-18.0 render: the terminal rises out of the editor pane. The command is typed, the real output prints, and the progress bar and frame counter run while the player's playhead runs with them. At "Render complete" the panes clear and the player shrinks into one film cell at centre.
4. 18.0-24.0 same: the cell grows into filmstrip A, and strip B whips in from the right with the identical frames. B decelerates into x alignment, then both converge vertically onto one line at 3.4 (the payoff, about 71%). "Same input." becomes "Same frames.".
5. 24.0-30.0 end: the strip collapses to the centre. The two symbol halves arrive from left and right and lock, the wordmark wipes in, the tagline lands, then `$ npx skills add heygen-com/hyperframes` types out and holds 2.5 s.

BANNED: the spec defaults (dark void, glow, purple gradients, glass, cream with serif, fade-and-slide-up, 3 cards, docked logo, corner labels), plus pill chips around the command, a timecode readout, and any claim of render speed.

QA: frames 0, 1.0, 2.9 / 3.0 (seam), 4.5, 7.0, 8.8, 11.0, 13.5, 16.0, 17.9 / 18.0 (seam), 21.5, 23.9 / 24.0 (seam), 27.0, 29.9.
