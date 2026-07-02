# Color Story

Color Story is a single-page palette maker for naming colors, writing stories, saving work locally, and sharing or backing up the result. It's designed with elementary-school users in mind: friendly toast messages instead of browser alerts, generous line-break support, and simple stepper controls.

## Features

- Create a custom grid from 1×1 to 10×10 using compact +/− stepper buttons.
- Set the card border thickness while editing a palette.
- Edit each card's color name and story directly on the card with borderless, auto-resizing fields.
- Write multi-line names and stories — press Enter to add a line break, both on-card and in the detail modal.
- Open detailed color controls from a card-only action button that appears after selecting a card.
- Friendly toast notifications and a custom confirm dialog (with emoji) replace plain browser alert/confirm popups.
- A first-use tip banner reminds new users to tap a card to start writing, and hides itself once a card is filled.
- Preserve line breaks everywhere: on-screen, in exported images, copied text, and share links.
- Save palette state in browser local storage so refreshes do not erase work.
- Export as an image, copy text, create a compressed share link, or use the top-right disk menu for JSON backup/restore.
- Switch between Korean, English, and Japanese.
- Use dark/light mode and mobile-friendly controls.
- Show a full-grid notice and offer an add-row action when every card is filled.

## Usage

1. Open `index.html` in a browser.
2. Choose columns and rows with the +/− steppers, then tap "시작하기" (Start).
3. Type names and stories directly into cards — Enter creates a new line.
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
