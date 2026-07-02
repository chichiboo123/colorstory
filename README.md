# Color Story

Color Story is a single-page palette maker for naming colors, writing stories, saving work locally, and sharing or backing up the result.

## Features

- Create a custom grid from 1×1 to 10×10.
- Set the card border thickness before or after creating a palette.
- Edit each card's color name and story directly on the card with borderless fields.
- Open detailed color controls from a card-only action button that appears after selecting a card.
- Preserve line breaks in story text.
- Save palette state in browser local storage so refreshes do not erase work.
- Export as an image, copy text, create a compressed share link, or use the top-right disk menu for JSON backup/restore.
- Switch between Korean, English, and Japanese.
- Use dark/light mode and mobile-friendly controls.
- Show a full-grid notice and offer an add-row action when every card is filled.

## Usage

1. Open `index.html` in a browser.
2. Choose columns, rows, and border width, then create the grid.
3. Type names and stories directly into cards.
4. Click a card to reveal the details button, then adjust its color if needed.
5. Use the top-right disk icon to choose backup or restore.

## Development

No build step is required. To serve locally:

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000` in your browser.

## Storage

Palette data is stored in the browser's local storage. Use JSON backup for important palettes because browser data can be cleared by private browsing, cache cleanup, or switching devices.
