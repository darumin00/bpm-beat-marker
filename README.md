# BPM Beat Marker Generator for DaVinci Resolve

A free web tool that puts beat markers on your DaVinci Resolve timeline — including the **free version** of Resolve.

Type in the BPM of your song, and the tool generates a marker EDL file you can import straight into Resolve. Bar starts (every 4 beats) are marked in red, the other beats in blue.

**Use it online:** open `index.html` in a browser, or visit the GitHub Pages site for this repository.

## How to use

1. Enter the BPM, frame rate, and song length
2. Download the generated `.edl` file
3. In DaVinci Resolve, right-click your timeline in the Media Pool → **Timelines → Import → Timeline Markers from EDL**, and select the file

If the song starts partway into the timeline, set the offset to the song's start position in seconds.

## Features

- Markers on every beat (interval can be set to every 1 / 2 / 4 / 8 / 16 beats)
- Frame rates from 24 to 120 fps (including 60 and 120)
- Offset to the first beat, custom timeline start timecode
- 8 languages: 日本語 / English / Español / Deutsch / Français / Português / 한국어 / 简体中文 — your language choice is remembered
- No install, no sign-up

## Limitations

- The BPM is not detected automatically — you need to know your song's BPM (sites like Tunebat list it for most songs)
- Drop-frame timecodes (29.97 fps etc.) are not supported (calculated as 30)

## Privacy & safety

The whole tool is a **single HTML file** (`index.html`). Everything runs locally in your browser: no server, no uploads, no tracking, no accounts. You can read the entire source in this repository — what you see is exactly what runs. If you prefer, download `index.html` and open it offline; it works forever with no connection.

## License

MIT
