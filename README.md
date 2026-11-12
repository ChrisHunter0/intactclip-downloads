# IntactClip — downloads

Binary releases only. **Source code is not published in this repository.**

| Platform | File | Notes |
|---|---|---|
| Windows 10/11, 64-bit | `intactclip-win64.zip` | Unpack anywhere, run `intactclip.exe`. No installer, no admin rights. |
| macOS 12+, Apple Silicon | `intactclip-macos-arm64.zip` | Experimental. Unsigned and not notarized — see below. |

Download the zip from the [latest release](../../releases/latest). Do **not** use the
"Source code" archives that GitHub attaches automatically: they do not contain a runnable
build.

## First run

**Windows** — the build is not code-signed yet, so SmartScreen shows
"Windows protected your PC". Click **More info → Run anyway**. The app opens
`http://127.0.0.1:8765/` in your default browser; all processing happens on your machine.

**macOS (Apple Silicon)** — the app is unsigned and not notarized. After unpacking, run
`start.command` from Terminal, or right-click the app and choose **Open**. macOS may ask you
to confirm in **System Settings → Privacy & Security → Open Anyway**.

## What is inside

- `intactclip.exe` (Windows) or the bundled app (macOS), plus the Python runtime it needs
- `ffmpeg` / `ffprobe` — an unmodified third-party build, invoked as a separate process
- `LICENSE.txt` — IntactClip end user license
- `ffmpeg-LICENSE.txt` and `FFMPEG-SOURCE.txt` — GPL v3 text and the exact build
  provenance, including where the corresponding ffmpeg source can be obtained

## Free tier

The build is the full program. The free tier allows a limited number of trial tasks, then
per-task limits on clips, files and merge segments; frame-accurate re-encoding is limited to
a few trial uses. A one-time license removes those limits. No subscription, no account, no
uploads.

## Support

Open an issue here, or write to `support@getintactclip.com`.
