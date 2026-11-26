# Private Garden levels and solutions

The levels of the puzzle games *Private Garden* (levels 01 to 150, and the special levels cho-muzu01 to
cho-muzu12), *Private Garden 2* (pg2-001 to pg2-231) and *Private Garden 3* (from pg3-001), decoded from screenshots,
each with its best known solution.

- `levels/NAME.txt`: a level.
- `solutions/NAME-solver.txt`: its best known solution, played through in the game. Its second line says how it was
  found and whether it is proven shortest.
- `solutions/NAME-WHAT.txt`: an alternative (a longer route, the hint's route, an earlier solution); its header says
  what it is an alternative to.

A move is one input: a whole glide or roll counts as one move.

`HANDBOOK.md`: the game's rules, the habits that make solving work, and the notation, for a reader learning the game.

## Level files

Sections, each under its own heading line, rows written from the top of the board down:

- `ground`: one character a cell. `#` wall, a space outside the board, `.` floor, `_` ice, `O` pit, `1` `2` `3`
  damaged floor (`3` the last stage, rubble), `4` `5` `6` damaged ice (`6` the last stage), `@` a warp (two in a
  level, sending a piece to each other), `?` ground hidden under a piece that never moves.
- `pieces`: each piece its own letter on every cell it covers, `.` elsewhere. A piece wholly over pits is down in
  them (fallen); one with any block on ground is held up by it.
- `fallen` (pg2-114, pg3-001): a second grid like `pieces`, for a piece lying in a pit under another.
- `legend`: piece letters to kinds: `girl1` to `girl7` (one a colour), `male`, `car`, `ball`, `iceball`, `gay`
  (a gay tile), `bomb1` to `bomb9` (Private Garden 3: a bomb showing that count; it counts down with each of its
  own moves, and showing 1 it goes one cell, on ice or not, and explodes there, leaving a pit).

Girl colours: girl1 brown-haired (in Private Garden 2 Mikan, orange frame), girl2 blonde (Biwa, cyan), girl3
dark-haired (Kurumi, green), girl4 pink-haired (Momo, pink), girl5 tanned (Karin, pale yellow); in Private Garden 3
also girl6 Lemon (white frame) and girl7 Saya (blue).

## Solution files

One move a line: the piece's kind letter, one of its cells as `x y`, and a direction `U` `D` `L` `R`.

- Kind letters: `F` girl1, `G` girl2, `K` girl3, `J` girl4, `N` girl5, `S` girl6, `T` girl7, `M` male, `C` car,
  `B` ball, `I` ice ball, `H` gay tile, `1` to `9` a bomb showing that count.
- Cells: `x` the column from the left edge, `y` the row from the bottom edge, both counted from 0 at the grid's edge.
  With the walls on the edges, `x` is the chessboard file (A = 1) and `y` the rank: `3 6` is C6.
- Lines starting with `#` are comments. The first, `# level NAME, board HEX`, ties the file to its level's board.

Example, level 06 (5 moves): `F 3 6 D` moves the girl pair on C6-D6 down one cell.
