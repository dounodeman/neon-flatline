# NEON FLATLINE

A top-down cyberpunk arena survival game that runs in the browser. Chrome up, hack the gangs, and survive the rain-soaked streets of Vanta City without losing your humanity.

Everything is one `index.html`: HTML5 Canvas, vanilla JavaScript, and Web Audio. The music, sound effects, neon signs, and rain are all generated in code, so there are no image or audio files.

## Play

Open `index.html` in a modern browser (Chrome, Edge, Safari, Firefox). Fonts load from Google Fonts. Without a connection the game still works and falls back to system fonts.

## Controls

| Input | Action |
| --- | --- |
| `WASD` / arrows | Move |
| Mouse | Aim / attack (hold to keep attacking) |
| `1`–`4` / mouse wheel | Katana · Smart SMG · Thermal Shotgun · Monowire |
| `Shift` | Dash (brief invulnerability) |
| `Space` | Sandevistan: time slows to 0.2x |
| `Tab` (hold) | Optics scan: slows time and shows enemy intel |
| `Q` / `E` / `R` | Quickhacks: Short Circuit · Overheat · Cyberpsychosis |
| `B` | Ripperdoc clinic (pauses the game) |
| `P` / `Esc` | Pause |
| `M` | Mute |

## Features

- **Five gang factions plus a boss.** Chrome Jackal rushers, Neon Oni blade-dashers, Kurogane gunners with laser sights, Ghostwire netrunners that hack you, and Meathook bruisers. Every fifth wave brings a cyberpsycho with charge attacks, shockwaves, and an enraged phase.
- **Netrunner traces.** An enemy netrunner uploads a hack to your deck over a visible data line. Hit it before the upload finishes, or your motor functions jam.
- **Quickhacks with upload time.** Short-circuit, set enemies on fire, or turn them against each other.
- **Katana deflects bullets** back at the shooters.
- **Humanity system.** Every cyberware implant costs humanity. Low humanity boosts your damage, but it also brings glitches, hallucinations, and eventually cyberpsychosis. Braindance therapy buys some of it back.
- **Atmosphere.** Neon signs that flicker (and sometimes break), rain that freezes mid-air during the Sandevistan, puddle reflections, steam vents, police AV searchlights, CRT scanlines, chromatic aberration, and glitch post-processing.
- **Procedural darksynth soundtrack.** It slows down and muffles during Sandevistan and when you visit the ripperdoc.
- **Fixer briefings and radio chatter** that introduce each new threat.

## Tech notes

- The simulation runs on a fixed 60 Hz timestep, so game speed doesn't depend on your monitor's refresh rate.
- The 1280×720 stage scales to fit the window, with a high-DPI backing canvas.
- Your best run is saved in `localStorage`.
