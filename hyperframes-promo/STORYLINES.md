# HyperFrames promo: three storylines

**The one thing:** you write HTML, and HyperFrames renders it to video, the same frames every time.
**What the viewer remembers:** "My video is just a web page I can edit."
**Source of every claim:** the repo README ("Write HTML. Render video. Built for agents.", open source under Apache 2.0, deterministic MP4, no React required, `npx skills add heygen-com/hyperframes`), the real CLI output and the logo in `docs/logo/`.

Assumptions: 28–34 s, 1920×1080 at 30 fps, music bed plus a few sound effects, no voiceover. Music comes from the HeyGen catalog only if you're signed in. You aren't now, so the free path is a local or royalty-free track you supply; without one I'll deliver it silent and say how to add music. Nothing paid.

---

## A. The file is the film (recommended: it shows the real mechanism using only real artifacts I can capture here)

- **Device / form:** the result first; one continuous take that keeps pulling back.
- **What the viewer sees and feels:** a bold title is already moving full-frame. The camera pulls back to show it's a video, then pulls back again to show that the video is an `index.html` file. One line of CSS changes and the video changes with it, then it renders to an MP4. The feeling is "oh, it's just code."
- **First two seconds:** full-frame kinetic type "Write HTML." lands word by word on a saturated brand-colour ground, with frame 0 already showing "Write".
- **Beats:** hook (the title playing) → pull back to the player with a timeline scrubbing → pull back to the editor showing the real `index.html` beside it (reveal: "It's just HTML") → proof: edit `font-size`, the title grows in the player, then scrub and see the same frame every time → `npx hyperframes render` progress fills and `video.mp4` lands (payoff, 70%) → claim "Write HTML. Render video." → end card: the logo is wiped in, then `npx skills add heygen-com/hyperframes`.
- **Look:** a light editor surface for the "home" world and the brand colour for the video world, set in the bundled sans with monospace only inside real code. The one treatment is the frame border of the player, which becomes the editor pane.
- **Sound:** a clean pulse around 110 bpm that stays thin until the render, then opens at the MP4 landing. Key ticks on the CSS edit, one whoosh per pull-back (two takes rotated) and a riser into the logo.

## B. Change one word

- **Device / form:** one viewer doing one task, in an object-to-object chain.
- **What the viewer sees and feels:** someone asks their coding agent for a launch video, and a real editable project appears. They mark one word in the title, ask for a change and only that word changes. The feeling is control: it isn't a black box.
- **First two seconds:** a finished launch frame with one word circled by a large cursor, and the caption "Change just this word."
- **Beats:** hook (the circled word) → tension (a regenerate button reshuffling everything, the old way) → reveal "HyperFrames" → proof: ask, project appears, mark, change → payoff: the edited video plays → claim → end card.
- **Look:** follows the Studio app's own UI. This needs **real Studio screenshots that I can't capture here**, so without them those shots become labelled placeholders.
- **Sound:** a warm mid-tempo bed, a real click on every cursor click and pops when the word swaps.

## C. Same input, same frames (the bold one)

- **Device / form:** type carries the argument, cut on the beat.
- **What the viewer sees and feels:** giant kinetic type built out of real code tokens. `<div class="clip">` breaks apart into pixels that stack into a filmstrip, and a frame counter (0001 → 0900) runs twice with the strips matching exactly. The feeling is that this is precise and engineered.
- **First two seconds:** a full-frame code line `data-start="0"` whose `0` swells into a frame counter.
- **Beats:** hook (code becomes a counter) → "Write HTML." → "Seek every frame." → two filmstrips rendered side by side snap together as identical (payoff) → "Open source. Apache 2.0." → end card.
- **Look:** a high-contrast two-colour field cut every half beat, oversized sans type and code in mono. The one material is the filmstrip.
- **Sound:** a driving 124 bpm electronic track where every cut lands on the beat, with a single impact when the strips match.
