# Soundroom

A lightweight, Spotify-inspired music player for personal use.

## Features
- Import browser-supported audio files (MP3, WAV, M4A, OGG, and others) into a local IndexedDB library for later playback on the same browser/device.
- Search, play/pause, next/previous, shuffle, repeat, seek, and volume controls.
- Load official Spotify embeds for supported track, album, playlist, episode, and show links.
- Responsive layout; no build step or API key required.

## Important limitation
Spotify embeds still load from Spotify's own services. This app does not proxy Spotify, download Spotify streams, or bypass a school's network restrictions. If Spotify is blocked by the network, the embed may not load. The local library works with audio files you have permission to use.

## Run locally
Open `index.html` in a modern browser. For the most reliable IndexedDB behavior, serve the folder from a local static server, for example `python3 -m http.server 8000`, then open `http://localhost:8000`.

## Deploy
This is a static site and can be hosted with GitHub Pages or another static host. Hosting the page does not change whether Spotify's own services are reachable from a given network.

## Privacy
Imported audio is stored in this browser's local IndexedDB database. Clearing browser site data may remove it. Audio files are not uploaded to a server by this app.

Soundroom is an independent project and is not affiliated with Spotify.
