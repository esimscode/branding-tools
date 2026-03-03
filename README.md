# LiveCultr — Email Signature Generator

A lightweight, zero-dependency email signature generator for the LiveCultr brand. Fill in your details, get a live preview, and copy a signature ready to paste into Gmail, Outlook, or Apple Mail.

## Features

- **Live preview** — signature updates as you type
- **Gmail-ready copy** — copies rich HTML that pastes directly into Gmail's signature editor
- **HTML copy** — for Outlook, Apple Mail, and any client with an HTML signature mode
- **Profile photo support** — paste any image URL for a circular avatar
- **Social links** — LinkedIn and X (Twitter) icons included
- **No build step** — open `index.html` in a browser and go

## Files

| File | Purpose |
|------|---------|
| `index.html` | The signature generator (form + live preview + copy buttons) |
| `signature.html` | Static HTML preview of the signature template |

## Usage

1. Clone or download this repo
2. Open `index.html` in any modern browser
3. Fill in your name, title, email, phone, photo URL, and social links
4. Click **Copy for Gmail** to paste into Gmail Settings → Signature, or **Copy Signature HTML** for Outlook/Apple Mail

No server, no npm install, no dependencies.

## Installing in Gmail

1. Click **Copy for Gmail** in the generator
2. Open Gmail → Settings (gear icon) → **See all settings**
3. Under the **General** tab, scroll to **Signature**
4. Create or edit a signature and paste (`Cmd+V` / `Ctrl+V`) directly into the editor

## Installing in Outlook / Apple Mail

1. Click **Copy Signature HTML**
2. In your email client, open the signature editor in **HTML mode**
3. Paste the copied HTML

## Customization

The generator is a single self-contained HTML file. To adapt it for a different brand:

- Colors: search for `#F27866` / `#FED0AB` (the LiveCultr gradient) and replace with your palette
- Logo: swap the inline SVG in `LOGO_SVG` at the top of the `<script>` block
- Company name/URL: update `livecultr.co` references in `buildSignatureHTML()`

## License

MIT
