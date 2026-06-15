# Repository Guidelines

## Project Structure & Module Organization

This repository is a self-contained HTML5 canvas game. The primary source is `index.html`, which contains the markup, styles, and embedded JavaScript for the full game. `README.md` gives quick run instructions, and `PROJECT_CONTEXT.md` records current project assumptions and gameplay notes for future work. `outputs/skyfront-1949.html` is a previous generated copy; treat it as reference output unless a task explicitly asks to update it. Keep new assets or generated exports under clearly named folders, and avoid splitting `index.html` unless the change intentionally introduces a build structure.

## Build, Test, and Development Commands

- `npm start`: starts a static server on port `5174` with `python3 -m http.server`.
- `npm run check`: extracts inline `<script>` blocks from `index.html` and validates that they parse as JavaScript.

You can also open `index.html` directly in a browser for a quick manual check. Avoid port `5173`; project notes indicate it is already used by another local app.

## Coding Style & Naming Conventions

Follow the existing single-file style in `index.html`. Keep indentation consistent with nearby code, use descriptive names for gameplay state and UI helpers, and group related constants, rendering logic, input handling, and update loops together. Prefer small, focused changes over broad rewrites. Since the game is browser-only, avoid adding dependencies unless they clearly reduce complexity and are documented in `package.json`.

## Testing Guidelines

Run `npm run check` after every code change. For gameplay changes, also perform a manual browser pass at `http://localhost:5174/`: verify startup, account/profile selection, keyboard controls, touch controls when relevant, and the specific mode or feature you changed. There is no automated coverage framework yet, so document any manual test coverage in the pull request.

## Commit & Pull Request Guidelines

This checkout does not include Git history, so commit conventions cannot be inferred locally. Use short, imperative commit messages such as `Fix boss collision timing` or `Add aircraft upgrade preview`. Pull requests should include a concise summary, the reason for the change, test results such as `npm run check`, and screenshots or short recordings for visible gameplay or UI updates. Link related issues when available.

## Agent-Specific Instructions

Keep edits focused in `index.html` unless the task calls for project restructuring. Preserve the browser-local save model based on `localStorage`. Do not modify generated output files unless requested.
