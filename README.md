# Playroom

A personal game library with search, platform and genre filters, favorites, recent history, and an integrated player.

## Open the library

Open the single `index.html` file in a modern browser. The interface is self-contained; selecting a game downloads its compressed game page from this repository. The original game pages may also request assets from their original external hosts.

## Collection

- 1,269 HTML5 game pages
- 437 Flash game pages
- 1,142 emulated game pages
- 2,848 game pages in total

Nineteen emulator templates and one non-game document are excluded. All supplied game pages are retained, including variants. 344 broken Flash movie URL placeholders were repaired. Game code runs in a sandboxed player; unavailable external assets and individual browser compatibility can still prevent some games from running. Catalog inclusion does not certify that every game has been play-tested.

## Storage

`game-data/` contains gzip-compressed HTML, split into at most 16 MiB binary pieces. The pieces for each game form one gzip stream. The catalog embedded in `index.html` records paths, lengths, and SHA-256 checksums. Only the selected game is fetched; the entire collection is never downloaded at startup.

The GitHub Pages workflow publishes only `index.html`; game data is served from this repository separately. This keeps the published Pages site small. The same HTML can be downloaded and opened locally.

## Credits

Game content belongs to its respective authors and rights holders. This repository does not grant new licenses to third-party game content. Decorative cover illustrations are not game screenshots. Favorites and play history are stored locally in the user's browser.
