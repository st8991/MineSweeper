# MineSweeper

A Minesweeper clone written in Java Swing for CS 251.

Pick a difficulty, then clear the 16×16 board without stepping on a mine. Flag every mine to win; the game shows how long you took.

## Features

- 16×16 grid with three difficulty levels: Easy (8 mines), Normal (16) and Hard (32)
- Numbered cells colored by how many mines touch them
- Automatic flood-fill reveal when you open a cell with no neighboring mines
- Remaining-mine counter in the title bar
- Win timer and a game-over message when you hit a mine

## Controls

| Action | Input |
| --- | --- |
| Reveal a cell | Click |
| Flag a cell as a mine (`@`) | Ctrl + click |
| Remove a flag | Alt + click |

## Run it

Requires a JDK (8 or newer). The classes live in the `game` package, so compile them into a `game` folder:

```bash
javac -d out *.java
java -cp out game.MineSweapPart
```

## Project layout

```
MineSweapPart.java       Game window, board setup, mine placement and click handling
MyJButton.java           A grid cell that remembers its row and column
DifficultySelector.java  Start-up dialog for choosing the difficulty
```
