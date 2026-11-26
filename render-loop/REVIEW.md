# REVIEW: How HTML becomes video (vertical loop)

## Creative calls

- The subject is how HyperFrames renders. You picked "Explainer loop" without naming a topic, so I used the example given in that option.
- Every step comes from `docs/concepts/determinism.mdx`: frame clock (`time = frame / fps`), seek (timelines paused and seeked, never played), capture (Chrome), encode (FFmpeg).
- The worked example is frame 90 at 30 fps = 3.0 s. The page's 5 s length and the ball animation are illustrative.
- One scene, one continuous diagram, no cuts:
  - the counter becomes the equation;
  - "3.0 s" flies down to become the timeline label;
  - the page is captured into the filmstrip;
  - the strip collapses into video.mp4.
- It's a seamless loop: the closing beat returns the counter to 89, so the next pass rolls it to 90 again.
- It's silent, because loops autoplay muted in feeds.

## Measured vs looked at

- `lint` clean; `check` ok. Every readable element sits inside the TikTok / Reels / Shorts safe box (288–1248 px down, 120–840 px across).
- Rendered file: 1080×1920, 30 fps, 390 frames. The first and last frames differ only by compression noise (PSNR 54 dB).
- Looked at every beat on contact sheets plus a zoom on the file tile.

## Warnings kept on purpose

- `line_unread` on the closing counter and "Pick a frame.": in a loop, these run straight on into frame 0, so a viewer reads them for over 2 s across the loop point.
- `data-layout-ignore` on the counter's roll and tick row. Those elements are masked, and only their visible cells (checked by eye) sit in frame.

## Weakest beat / next

- Encode (8.9–10.6 s) is the most abstract: the strip runs and collapses, but nothing shows FFmpeg doing work. With more time, cells could stream into the file one by one while a frame counter ticks up.
