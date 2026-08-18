# Peggle Dual Shot

A self-hosted browser emulator built on [EmulatorJS](https://emulatorjs.org/) (MIT licensed).

## Structure

```
.
├── index.html      # Page that boots the emulator
├── .nojekyll       # Needed for GitHub Pages to serve everything correctly
├── data/           # EmulatorJS engine (loader, player, cores config)
└── roms/           # Put your NDS ROM file here
```

## Setup

1. Drop your `.nds` ROM file into `roms/`.
2. In `index.html`, update `EJS_gameUrl` to match your exact filename.
   (Spaces in filenames need to be written as `%20` since this is a URL, not a plain filesystem path.)
3. Push to GitHub, enable Pages (Settings → Pages → Source: `main` branch, root folder).

## Notes

- `EJS_core` is already set to `"melonds"` for Nintendo DS — no need to change it.
- If your file upload is over 25MB, GitHub's website uploader will block it — use GitHub Desktop or `git` from the command line instead (no such limit there, up to 100MB per file).
- Only load ROMs you actually own/have the rights to use.
