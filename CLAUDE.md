# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A collection of browser-based games and web apps, built as single self-contained HTML files (HTML + CSS + JS in one file). No build tools, no dependencies, no server required — everything runs by opening a file directly in a browser.

## Running the Project

Open any HTML file directly in a browser:
```
# Windows
cmd.exe /c start "" "C:\Users\claud\Desktop\ClaudeCodeTest\<file>.html"
```

## Git & GitHub Workflow

This repo is hosted at https://github.com/dimondsword/ClaudeCodeTest.

After every meaningful change, commit and push:
```bash
git add <file>
git commit -m "<clear, specific commit message>"
git push
```

Keep commit messages concise and descriptive (e.g. `"Add restart button to tictactoe"`, not `"update stuff"`).

## Architecture

Each project is a **single `.html` file** containing:
- Inline `<style>` for all CSS
- Inline `<script>` for all JS
- No external dependencies or CDN links

This pattern keeps projects portable and simple — do not introduce package managers, bundlers, or frameworks unless explicitly asked.
