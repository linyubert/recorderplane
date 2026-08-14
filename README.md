# Recorder Flight

A side-scrolling flight game controlled by a recorder. Blow Sol, La, Si or Do into the microphone and the plane climbs to that line or space on the staff, threading the gap in each oncoming wall.

Recorder Flight is part of **Dato Music Lab** (https://datomusiclab.dpdns.org), a working elementary music teacher's studio in Taipei.

## What it is

Students learn that Sol sits on the second line and La in the second space, and they can recite it long before they can *use* it. The gap is that staff position stays an abstract fact rather than a thing with consequences.

Here the staff is the playing field. Blowing a higher note lifts the plane to a higher line, so pitch, staff position and physical height are the same fact three times over. The wall gaps are labelled with note names, which means reading the staff is not a separate exercise — it is how you avoid crashing.

## Features

**Microphone pitch detection.** Autocorrelation on the recorder's fundamental, with automatic octave handling.

**A real staff.** Standard treble clef, with note positions that are musically correct rather than decorative.

**Hold to hover.** Sustain a note and the plane parks on that line, so a student can line up on the gap before reaching it instead of having to time a jump. The skill being tested is pitch, not reflexes.

**Three stages, thirty questions.** Reach question thirty and the mission is complete.

**Keyboard fallback.** `Z` `X` `C` `V` for anyone without a recorder to hand.

**Local leaderboard**, weather that changes by stage, crash effects, and win/lose sounds.

**Fills the screen**, suited to a large display.

## How to use

Download the folder and open `index.html` in Chrome, Edge or Safari. Grant microphone access when asked. If the notes are accurate but nothing responds, raise the sensitivity in the settings panel.

### Pitch to height

| Note | Staff position | Key | Colour |
|:---|:---|:---:|:---:|
| Sol (G) | Second line | `Z` | Yellow |
| La (A) | Second space | `X` | Teal |
| Si (B) | Third line | `C` | Pink |
| Do (C) | Third space | `V` | Purple |
| Re (high, D) | — | `B` / `Space` | Start or restart |

Sol and Si sit **on lines**; La and Do sit **in spaces**. Higher note, higher flight.

Stages run through clear skies, a thunderstorm, and dusk.

## Tech

Pure front end — HTML5 Canvas, Web Audio API and `getUserMedia`, with no framework or dependencies. The pixel typeface is Press Start 2P, falling back to a monospace face when offline.

```
index.html    The game; key art is embedded as base64
lose.mp3      Failure sound
win.mp3       Completion sound
```

## License

Code is MIT — see [LICENSE](LICENSE). Artwork and audio are original work by Yucheng Lin under separate terms; see [NOTICE.md](NOTICE.md).

## More from Dato Music Lab

The same pitch detection drives a fruit-slicing arcade game, where accuracy is rewarded with a clean cut and a visible tuner shows whether a student is sharp or flat. For reading rather than playing, there is a two-team sight-reading tug-of-war on a single touchscreen; for duration, a rhythm game about squeezing ketchup for exactly the length of each note. All at **https://datomusiclab.dpdns.org**.
