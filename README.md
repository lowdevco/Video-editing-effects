<div align="center">

# 51 Video Effects for Claude

This is a Claude Code skill that helps you add visual effects to your videos. It analyzes your footage, creates the requested effect, and saves an edited video while keeping the original audio.

Add your video to Claude, enter `/effects` followed by an effect name, and you're ready to edit.

Created by [@samknows.ai](https://www.instagram.com/samknows.ai)

<p align="center"><img src="assets/samknowsai.jpeg" alt="Profile picture of the skill provider" width="500"></p>

## Install (one command)

Open Terminal, or the terminal in Claude Code, and run:

```bash
git clone https://github.com/lowdevco/Video-editing-effects.git ~/.claude/skills/effects
```

In Windows PowerShell, replace `~/.claude/skills/effects` with `$HOME\.claude\skills\effects`.

Restart Claude Code when the command finishes.

> Need a hand? In Claude Code, paste: **"Install the skill from github.com/lowdevco/Video-editing-effects.git into ~/.claude/skills/effects"**. Claude can install it for you.

## Use it

1. Launch Claude Code, either the app or the terminal.
2. Add your video to the chat by dragging it in.
3. Enter the effect you'd like to use:

```
/effects orbit from 3 to 6 seconds
/effects spotlight when I say "kill the lights", with the word Claudit behind me
/effects comment-box at the end, typing CLAUDE
/effects glass-widgets for the first 3 seconds
```

On first use, setup takes about two minutes. Claude needs `ffmpeg` and Python, and will install either one if it's not already available.

Claude first reviews a few frames and adjusts anything that obscures your face. It then saves `yourvideo_effects.mp4` beside the original video, keeping the original audio.

Combine effects in a single request, for example: *"Add locked-on from 6 to 10s, then orbit from 10 to 13s, then a reject stamp on 'no'."*

## The 51 effects

| # | Type this | What happens |
|---|---|---|
| 1 | `noise` | Reels pile up behind your head |
| 2 | `lineup` | Numbered tiles fan out above your head |
| 3 | `locked-on` | Brackets lock onto your face and the camera follows you |
| 4 | `orbit` | Your reels circle your head, behind you at the top |
| 5 | `lean-in` | A quick punch-in on one word |
| 6 | `backdrop-word` | A giant word drops in behind you |
| 7 | `spotlight` | Kill the lights, keep you lit |
| 8 | `the-bill` | Your instructions print out like a receipt |
| 9 | `moody` | A moody colour grade |
| 10 | `swipe` | A before and after slider |
| 11 | `todo` | A checklist beside your head that ticks off as you talk |
| 12 | `comment-box` | An Instagram comment types itself and posts |
| 13 | `tap` | A Follow button flips to Following |
| 14 | `pause-point` | Freeze frame with a hand-drawn arrow |
| 15 | `uninstall` | A glitchy uninstall bar breaks the frame |
| 16 | `reel-frame` | Your video shrinks into a reel card |
| 17 | `shortcut-rain` | Keyboard keys rain down behind you |
| 18 | `reject-stamp` | A big red stamp slams down |
| 19 | `countdown-flip` | A 3, 2, 1 flip clock above your head |
| 20 | `rabbit-hole` | The room tunnels away behind you |
| 21 | `cover-star` | You become a magazine cover |
| 22 | `scribble` | Marker doodles draw themselves around you |
| 23 | `glass-widgets` | Frosted glass widgets and mini artifacts float around your head |
| 24 | `red-collage` | Black and white you, a giant red word behind, three lines slam in |
| 25 | `split-headline` | A headline card slides down and pushes you to the bottom half |
| 26 | `pastel-word` | Lavender room, a giant word behind you, a profile card gets followed |
| 27 | `check-pills` | Grid-paper room, your reels pinned behind you, blue pills get clicked |
| 28 | `timeline` | A dark red film look with an editing timeline and a glowing playhead |
| 29 | `headline-box` | A punch-in with a clean two-line headline |
| 30 | `profile-wall` | Your reels grid fills the wall while a counter ticks up |
| 31 | `tier-list` | A tier list drops in and Claude flies into S tier |
| 32 | `broll-split` | B-roll on top with a price-tag sticker, you below |
| 33 | `phone-fan` | Your reels fan out like a hand of phones |
| 34 | `dot-reveal` | Your shot builds out of glowing dots, then snaps into focus |
| 35 | `headline-wall` | Your headlines pile up behind your head, then a total pops in front |
| 36 | `checklist` | A Claude task list under your chin, each step ticks green |
| 37 | `liquid-glass-graph` | A liquid glass card with a graph that climbs and a number that counts up |
| 38 | `carousel-spin` | Your reels spin around you in a 3D carousel |
| 39 | `match-cut` | News pages cut on one word, locked in place behind your head |
| 40 | `apple-toggles` | iPhone switches flip on under your chin, one line at a time |
| 41 | `led-sign` | The lights drop and a glowing LED sign types itself out behind you |
| 42 | `slow-push` | A slow cinematic push-in while the room melts out of focus |
| 43 | `over-the-shoulder-zoom` | Pushes into one corner, a liquid glass graph pops beside your head, then the other corner with a second graph |
| 44 | `messages` | iMessage notifications pop in one after another with a soft glow |
| 45 | `place-in-grid` | You shrink into the centre of your 3x3 profile grid, your reels pop in around you with view counts |
| 46 | `tape-label` | A strip of yellow tape with your line lands on your chest |
| 47 | `select-resize` | A blue selection box grabs your number and a cursor drags it bigger |
| 48 | `wave-trim` | The silent parts of your voice are trimmed away on screen until only your words are left |
| 49 | `huge-strike` | One huge serif word fills the wall behind you, then a red line crosses it out |
| 50 | `crayon-write` | A red crayon writes your word behind your head, then underlines it |
| 51 | `fan-build` | Your reel covers deal into a fan behind your head, one card at a time |

Bonus styles: `/effects glitter-spotlight` (golden rays and sparkles), `cover-star look=editorial` (a classic magazine cover), and `liquid-glass-graph look=bento` (a glass dashboard around you).

All effects track your face. Elements that might obscure it are placed behind your head instead.

**Tips**
- Vertical phone footage with you visible tends to work best.
- Describe timing conversationally (for example, "when I say 'watch'"). Claude finds the matching moment.
- To use your own reels in `orbit`, `noise`, `phone-fan`, or `profile-wall`, provide Claude with a folder of screenshots.
- Provide your actual figures for charts, counters, and headlines.
- Output is 1080p by default. You can request 4K, though rendering will take longer.

## A few notes
- These are **starter versions** and won't reproduce my reel exactly; that edit also uses sound design and carefully tuned timing.
- Claude creates a draft for you to review. Check the finished video before posting.
- Effects don't add sound or captions. You can add those in CapCut.
- Follow [@samknows.ai](https://www.instagram.com/samknows.ai) for updates.

## If something goes wrong
Describe the issue to Claude (for example, "the word covers my face" or "it's too fast"). Claude can adjust the plan and render again.

## Credits
Face tracking: [OpenCV YuNet](https://github.com/opencv/opencv_zoo) (MIT). Person cut-out: [MediaPipe Selfie Segmenter](https://ai.google.dev/edge/mediapipe/solutions/vision/image_segmenter) (Apache 2.0). Fonts: Archivo Black, Instrument Serif, Space Mono, Inter, Anton, Montserrat (SIL OFL) and Permanent Marker (Apache 2.0); licences are in `fonts/`. Everything else: MIT, see `LICENSE`.

</div>
