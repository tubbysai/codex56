# Nines

A responsive, single-player browser card game played against a computer opponent.
The entire game is implemented in `index.html`, with no build step or runtime
dependencies.

## Play locally

Open `index.html` directly, or serve the directory with a small local server:

```bash
python3 -m http.server 4173
```

Then visit <http://localhost:4173>.

## Rules

- Each player receives nine face-down cards in a 3-by-3 grid.
- Reveal two cards to begin, then draw from the deck or take the discard on each
  turn and replace one card in your grid.
- Number cards score their face value, aces score 1, jacks and queens score 10,
  kings score 0, and jokers score -2.
- A horizontal row of three matching ranks scores 0.
- When one player reveals their full grid, the other receives one final turn.
  The lowest final score wins.

## Copyable single-file version

`nines.html` is a complete copyable version of the game. Download or copy that one
file, save it with an `.html` extension, and open it directly in a browser. Its
HTML, styling, and game logic are all contained in the file.
