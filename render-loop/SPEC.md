# SPEC: How HTML becomes video (vertical explainer loop)

GOAL: in one 13 s loop the viewer gets the whole render model: pick a frame, turn it into a time, seek, capture, encode. Same frame, every time.
OUTPUT: HyperFrames, 1080 x 1920, 30 fps, seamless loop (the last frame equals frame 0).
TIME: 13 s x 30 = 390 frames. Silent: made to autoplay muted in a feed.
SOURCE: docs/concepts/determinism.mdx (frame clock `time = frame / fps`, seek with paused timelines, Chrome capture, FFmpeg encode). Frame 90 at 30 fps is the worked example; 5 s is an illustrative page length.

LOOK:

- Ground #f2f0ed, ink #181716, secondary text #57534e / #78716c, accent mint #3CE6AC (the highlighted frame, the page under capture, the file's band).
- Type: Inter 900. Step lines 84 px; counter 340 px; equation 110 / 220 px; small labels 36-44 px. JetBrains Mono for time labels and the file name.
- Everything readable sits inside the platform-safe box: 288-1248 px down, 120-840 px across (120-780 below 840).

OBJECTS: a frame counter with a tick row of neighbouring frames; the equation; a browser window whose page holds one ball animated over 5 s; a timeline track with a playhead; a filmstrip; an MP4 file tile.

MOTION: arrivals expo.out / power4.out; moves power3.inOut; exits power3.in. Step lines blur in per line (8 -> 0 px, 0.18 s); a landed line holds still.

SHOTS:

1. 0.0-2.2 "Pick a frame.": the counter rolls 89 -> 90 and the tick row steps one cell.
2. 2.3-4.5 "Work out the time.": 90 / 30 fps = 3.0 s.
3. 4.7-6.9 "Seek every animation.": "3.0 s" flies down to the timeline, the playhead seeks to it and the ball jumps to its 3.0 s position. Sub-line: "Paused. Seeked, never played."
4. 7.1-8.7 "Capture the pixels.": a flash, and the frame drops into its slot in the filmstrip.
5. 8.9-10.6 "Encode with FFmpeg.": video.mp4 opens with an empty band. The strip runs past the slot, and each of six frames lifts out of it and flies into the file, filling the band one sixth per frame. When the band is full, the play mark lands.
6. 10.8-13.0 "Same frame. Every time.": the counter returns at 89, then "Pick a frame." lands again, matching frame 0.

BANNED: the spec defaults, icons in circles, bullet slides, the whole diagram at once, numbered step labels, a logo end card.
