# ccnotify

Live data for the CCNotify Minecraft mod: clan name, whitelist, banner and the news panel's text.

The mod fetches `ccnotify.json` from this repo's `main` branch when the news panel is opened, and falls
back to the copy bundled in the jar if that fails. Edit `ccnotify.json` here and the change reaches
everyone without a new jar (raw.githubusercontent caches for a few minutes).

## news markup

One string per line in `news`:

- `# `, `## `, `### ` headers
- `- ` bullet
- `**bold**`, `*italic*`
- `&c`, `&a`, `&e`, ... vanilla colour codes, `&r` to reset
