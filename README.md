# EAGTC
Eastern Aries Galactic Trading Company

A C64-style real-time space freight game for the browser. Single file: open `index.html` in any modern browser. No build step, no dependencies (the pixel font loads from Google Fonts, with a monospace fallback).

## Play
1. Pick one of three freight contracts. Higher cargo value pays more and attracts more pirates.
2. Hire one alien department head for each station (6 candidates each):
   NAV (navigation), ENG (engineering/power), WPN (weapons), SCN (scanners), REP (repair).
   Skill, references and salary are shown. Temperament and quirks are only hinted at in the interview.
3. Choose jumps on the star map. Each leg runs in real time.
4. Press `1`–`5` to select a department, then `A`–`E` to set its priority. `P` pauses, `M` toggles sound.
5. Deliver the cargo. Profit = pay × cargo condition + bounties − dock fees − crew salaries.

Crew can panic (nervous), ignore orders (hothead), be injured or die. No replacements mid-trip.
A dead officer's station runs on weak automatic control.

## Encounters
| Map | Node | Counter |
|---|---|---|
| P | Pirate raiders | NAV evade/flee, ENG shields, WPN targeting, SCN analyze |
| A | Asteroid field | NAV evade, WPN asteroids, SCN rock track |
| X | Ion storm | SCN threat warning, REP |
| S | Repair dock | Auto repair, $250 fee |
| . | Quiet space | — |

Difficulty rises with distance and cargo value. High-profit list (top 10) is stored in the browser's localStorage.

## Status
Vertical slice. Keyboard only.
