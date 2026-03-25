# :moyai: Stone Face

Don't smile. Don't flinch. Don't raise an eyebrow. 60 seconds. 52 blendshapes watching your every micro-expression. Good luck.

## [Play Now](https://ashleywolf.github.io/stone-face/) (Chrome/Edge)

## What Is This

The only game where doing absolutely nothing is the goal. MediaPipe tracks 52 facial blendshapes while the game throws provocations at you for 60 seconds: jokes, weird emoji, distortion filters, sound effects. Any twitch drains your composure meter. The AI sees everything.

## Features

- 52 blendshapes tracked simultaneously: mouthSmile, jawOpen, browOuterUp, eyeSquint, cheekPuff, and more
- Fisher-Yates shuffled provocation order, so every playthrough hits different
- 23 taunts designed to make you crack (some are genuinely funny, which is the problem)
- Composure streak tracking with "ICE COLD" badge and regen bonus for staying flat
- Blendshape smoothing to filter out noise without letting real expressions slip through
- Countdown beeps in the final 10 seconds when you're most likely to break
- Win confetti + screenshot of your stone-cold victory face
- Emoji entrance animations that escalate in absurdity
- localStorage records so you can prove your poker face is improving

## How to Play

- Allow webcam access and calibrate your neutral face.
- Survive 60 seconds without reacting.
- Smiling, laughing, raising your eyebrows, opening your mouth: all drain composure.
- Maintain a streak of zero expression to earn the ICE COLD badge and composure regen.

## Tech

- MediaPipe FaceLandmarker with 52 blendshapes running in real-time
- Expression deviation calculated against calibrated neutral baseline
- Temporal smoothing to reduce false positives from lighting changes
- HTML5 Canvas with webcam feed and provocation overlay

## Browser Support

Chrome or Edge recommended. Requires webcam access. Performs best with consistent lighting so the model can distinguish your actual expressions from shadows.

## Part of Browser Party Games

8 single-file browser games built with MediaPipe, Transformers.js, Web Audio, and Web Speech. No servers, no build steps, no installs.

| Game | Input | Tech |
|------|-------|------|
| [Type or Die](https://ashleywolf.github.io/type-or-die/) | Keyboard | Vanilla JS |
| [Grin Sweeper](https://ashleywolf.github.io/grin-sweeper/) | Smile (webcam) | MediaPipe Face |
| [Show & Tell](https://ashleywolf.github.io/show-and-tell/) | Real objects (webcam) | Transformers.js DETR |
| [Pitch Climber](https://ashleywolf.github.io/pitch-climber/) | Voice pitch (mic) | Web Audio API |
| [Spell Caster](https://ashleywolf.github.io/spell-caster/) | Shout spells (mic) | Web Speech API |
| [Stone Face](https://ashleywolf.github.io/stone-face/) | Don't react (webcam) | MediaPipe Face |
| [Ninja Hands](https://ashleywolf.github.io/ninja-hands/) | Hand tracking (webcam) | MediaPipe Hands |
| [Duck & Cover](https://ashleywolf.github.io/duck-and-cover/) | Duck + yell (webcam+mic) | MediaPipe Pose + Web Audio |

---
Built with vanilla JS + browser ML. Each game is one HTML file. Fork it, break it, make it yours.
