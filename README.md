# OzoneGames

> A student games lab. No names. All skill.

## What This Is

OzoneGames is a curated, filterable gallery of browser-based games — some built by students, some built by teachers as demonstrations and starting points. It's a living portfolio for a classroom that treats game design as a legitimate programming discipline.

Every game is a standalone `.html` file. No frameworks, no login, no accounts. Drop a file in, add one entry to `games.json`, and it appears on the site.

## Why No Names?

The focus is on the work, not the identity. In a classroom context, anonymous publishing removes social anxiety around sharing unfinished or imperfect projects. Students can take risks they wouldn't take if their name was attached to every attempt.

When the work is strong enough that they *want* their name on it, they've leveled up.

## Adding a Game

1. Drop your `.html` game file into the `games/` folder.
2. Add an entry to `games.json`:

```json
{
  "id": "your-game-id",
  "title": "Your Game Title",
  "desc": "One sentence description.",
  "emoji": "🎮",
  "accent": "blue",
  "tags": ["puzzle", "one-button"],
  "madeByStudents": true,
  "file": "games/your-game.html",
  "notes": "Optional teacher notes about learning objectives."
}
```

3. That's it. The site handles the rest.

**Accent colors:** `cyan`, `red`, `blue`, `yellow`, `orange`, `green`, `pink`, `purple`

## Features

- Filter by All / Student Made / Teacher Made
- Collapsible teacher notes per game
- Sparkle hover effects (kids love these)
- Responsive grid layout
- Zero dependencies — pure HTML/CSS/JS

## Running Locally

Because `games.json` is loaded via `fetch()`, you need a local server:

```bash
# Python
python -m http.server 8080

# Node
npx serve .
```

On GitHub Pages it works without any setup.

## Tech

Pure HTML, CSS, JavaScript. No build step. Google Fonts (Fredoka, Inter). Lottie animations for decoration.

## Author

**Sean "Mook" DiMarco** — Creative Technologist, K–8 Educator  
EMPOW Studios (25 schools) · The Chestnut Hill School · Bowen After School  
Boston, MA | [sfdimarco.github.io](https://sfdimarco.github.io)
