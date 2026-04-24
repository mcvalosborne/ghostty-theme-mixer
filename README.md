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
2. Click **Copy command**
3. Paste the command into any terminal (Ghostty included) and hit enter — it appends to `~/.config/ghostty/config`
4. Reload Ghostty with `⌘ ⇧ ,` — change is instant, no restart

If a theme name isn't recognised by your Ghostty version, run `ghostty +list-themes | grep -i <name>` to find the exact spelling.

## Kept in sync with Ghostty

Theme keys in the mixer are verified **weekly** against [iTerm2-Color-Schemes/ghostty](https://github.com/mbadolato/iTerm2-Color-Schemes/tree/master/ghostty) — the upstream source Ghostty bundles its themes from. If a theme is ever renamed or removed upstream, a GitHub issue is opened automatically (see [`.github/workflows/check-themes.yml`](.github/workflows/check-themes.yml)) so the mixer stays in lockstep with whatever you have installed.

## Local development

It's a single static HTML file — no build step.

```bash
git clone https://github.com/mcvalosborne/ghostty-theme-mixer.git
cd ghostty-theme-mixer
open index.html
```

## License

MIT
