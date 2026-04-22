# Ghostty Theme Mixer

Live theme & font mixer for the [Ghostty](https://ghostty.org) terminal. Preview 16 color schemes and 4 coding fonts, nudge the background tint, and copy a ready-to-paste config in one click.

**→ [Try it live at ghosttythemes.com](https://ghosttythemes.com)**

![Ghostty Theme Mixer — live preview of terminal themes and fonts](screenshot.png)

## What's in it

- **16 themes** — four Gruvbox variants, Tokyo Night (+ Storm), Catppuccin (Mocha + Latte), Nord, Dracula, Rosé Pine, Solarized (Dark + Light), Kanagawa, Everforest, GitHub Dark
- **4 typefaces** — Fira Code, JetBrains Mono, IBM Plex Mono, Geist Mono
- **Background tint slider** — nudge any theme's background lighter or darker without losing the palette
- **One-click config** — copy the exact lines you need for `~/.config/ghostty/config`

## Apply your mix

1. Pick theme + font + tint in the mixer
2. Click **Copy config**
3. Paste into `~/.config/ghostty/config`
4. Reload with `⌘ ⇧ ,` in Ghostty — change is instant, no restart

If a theme name isn't recognised by your Ghostty version, run `ghostty +list-themes | grep -i <name>` to find the exact spelling.

## Local development

It's a single static HTML file — no build step.

```bash
git clone https://github.com/mcvalosborne/ghostty-theme-mixer.git
cd ghostty-theme-mixer
open index.html
```

## License

MIT
