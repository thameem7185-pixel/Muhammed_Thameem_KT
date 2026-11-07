# Muhammed Thameem KT | Portfolio

A fast, single-file portfolio for **Muhammed Thameem KT** (GitHub: [@thameem7185-pixel](https://github.com/thameem7185-pixel)), a web developer from Kozhikode, Kerala who builds AI chat apps, browser tools and ESP32 projects.

No build step, no framework, no dependencies. Everything lives in one `index.html`.

## Features

- **Two themes**
  - Dark: deep navy with Royal Azure (`#3D8BFF`) and cyan accents, with white highlights and a few small gold touches.
  - Light: a white page with forest green writing and soft green shapes drifting in the background.
  - A sun/moon switch in the top bar changes the theme and remembers your choice.
- **Hero** with a typing effect, a live node-network canvas that reacts to the cursor, floating skill chips and a profile ring.
- **Projects** shown as filterable cards (All, AI, Web, IoT, Education) with live previews and a link to each project.
- **Skills** with animated progress meters.
- **What I build with**: two moving banners, one for what I've built and one for tools and technologies. They use custom line icons, no emojis, and pause on hover.
- **About me**: one combined section with a photo card, the full story, "why work with me" points and an interactive journey timeline (2023 to now).
- **Contact** cards for email, location and social links.
- Scroll progress bar, scroll-spy navigation, reveal-on-scroll animations, back-to-top button.
- Responsive from small phones to desktop, keyboard-friendly, and respects `prefers-reduced-motion`.

## Project structure

```
index.html     the whole site (HTML, CSS, JavaScript)
profile.jpg    optional hero photo (falls back to "MT" initials if missing)
```

## Quick start

1. Download or clone the repo.
2. Open `index.html` in a browser. That's it.

## Customise it

All content sits in the `CONFIG` object near the top of the `<script>` block:

| Key | What it controls |
| --- | --- |
| `email`, `location` | Contact details |
| `roles` | Words in the hero typing effect |
| `social` | GitHub, LinkedIn and Instagram links (empty ones are hidden) |
| `skills` | Skill groups and percentages |
| `stack.row1`, `stack.row2` | Items in the two banners (see the `L` object in the script for icon names) |
| `projects` | Name, live URL, description, tags and an optional `image` |
| `journey` | Timeline entries |

### Colours

Colours are CSS variables at the top of the `<style>` block:

- `:root` holds the dark theme.
- `[data-theme="light"]` holds the light theme.

Change `--accent`, `--accent2`, `--bg`, `--ink` and the other variables to re-theme the site.

### Photo

- **Hero photo:** place a `profile.jpg` next to `index.html`.
- **About card photo:** it is embedded in the file as a base64 image. Replace the `src` of the `.hab-photo` image to change it.

## Deploy on GitHub Pages

1. Create a repo (for example `thameem7185-pixel.github.io`) and upload `index.html` (and `profile.jpg`).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. Your site will be live at `https://<username>.github.io/`.

## Notes

- Fonts (Sora, Inter, Archivo, Playfair Display) load from Google Fonts. Without internet, the site falls back to system fonts.
- Project preview images are fetched from free screenshot services. Set `image` on a project to use your own picture.
- The chosen theme is saved in the browser's `localStorage`.

## Built with

HTML, CSS and vanilla JavaScript, built in conversation with Claude.

## Contact

- GitHub: [thameem7185-pixel](https://github.com/thameem7185-pixel)
- Email: thameem7185@gmail.com
- Location: Kozhikode, Kerala, India
