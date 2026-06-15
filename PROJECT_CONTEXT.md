# Project Context

## Project

- Name: `giraffe1972`
- Type: single-page HTML5 canvas game
- Main file: `index.html`
- Previous generated copy: `outputs/skyfront-1949.html`
- Local dev port: `5174`

## How To Run

```sh
npm start
```

Open:

```text
http://localhost:5174/
```

## How To Check

```sh
npm run check
```

This validates the JavaScript embedded in `index.html`.

## Current Game Summary

This is a 2D aircraft shooting game inspired by classic vertical shooters. It includes:

- Account/profile selection stored in browser `localStorage`
- Tutorial flow for new accounts
- Modern war stages and void stages
- World War chapter with separate Allies and Axis aircraft pools
- Endless mode with score-based secret code hints
- Aircraft upgrades, bombs, specials, skins, achievements, codex, and boss previews
- Keyboard controls: WASD/arrow keys, Space for bomb, E/Enter for special, Shift for variable-wing mode where supported
- Touch controls for mobile devices

## Important Notes For Future Agents

- Keep edits focused in `index.html` unless intentionally splitting the project into multiple files.
- The game is currently self-contained, so moving or hosting it is simple.
- Save data is browser-local. Different browsers/devices do not share accounts unless a backend is added.
- Avoid using port `5173`; it is already used by another app on this machine.
- After code changes, run `npm run check`.

## Current Project Location

```text
~/Dev/giraffe1972
```
