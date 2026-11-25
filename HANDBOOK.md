# Private Garden: a handbook for solving levels

Everything needed to start solving Private Garden levels from scratch. It covers the rules as they were taught in
lessons 1-24, with their corrections folded in, the rules not taught yet, the habits that make solving work, and the
notation. The levels and their best known solutions are at https://github.com/quinyu/private-garden-levels (levels/,
solutions/; that repository's README explains the two file formats).

## Cells and directions

- Cells are named like a chessboard. Files A, B, C ... are the columns, counted from the first column inside the
  left wall. Ranks 1, 2, 3 ... are the rows, counted from the bottom row inside the walls. So B3 is the second column,
  third row from the bottom.
- **Up** means the row number grows (D2 → D3). **Down** means it shrinks (D3 → D2). Left and right change the letter.
- In lessons the board comes as a list of every cell by name, row by row ("row 6: A6 pit, B6 ice + girl, ..."), and
  also as a picture. Read the list: counting columns in a picture is easy to get wrong. If the two ever seem to
  disagree, the list is right.
- Damaged ground (Private Garden 2) is written in the list with the leavings it still bears: "cracked ice (2 left)"
  becomes a pit after two more leavings, a leaving being a piece leaving the cell or sliding across it.

## The rules taught so far (numbered as in the lessons)

**Goal and moves**
1. Goal: every girl disappears. Boys may be left over.
2. Contact: when a move ends with the boy right beside a girl (left, right, above or below, never diagonal), they
   vanish together.
3. A move: one piece, one direction (up, down, left, right).
4. On floor a piece moves exactly one cell.
5. On ice a piece slides (rule 23 says exactly how far).
6. Walls and standing pieces block: nothing moves into them.

**Girls sticking together**
7. A girl whose move ends beside a single girl of her colour sticks to her: a pair, lying (side by side) or upright
   (one above the other).
8. A pair is one piece: it moves as a whole, both blocks the same way, and never turns.
9. Two pairs that end as a 2x2 block stick into a square. A square never moves again. Sticking can chain within one
   move: a single sticks to a single, and the new pair at once sticks to a pair beside it into a square.
10. A single never sticks to a pair. A girl with two possible partners sticks to neither, and on ice she slides on.
17. Girls come in colours. Only girls of one colour stick; different colours never stick, even side by side.

**Clearing**
11. The boy clears every girl group he touches (single, pair or square) and vanishes with them. One boy makes one
    contact, so with one boy every girl must go in that one move: all of them in groups touching his last cell.
18. One contact clears every group the boy touches, whatever its colour.
22. In one move, sticking comes first, then contact. If the moved girl sticks into a bigger group and that group
    touches the boy, the whole new group vanishes.
25. Several boys: each boy makes his own one contact. The level is won when every girl is gone.

**Pits**
12. A piece that ends a move with every block over pits falls in. A single over a pit always falls in.
13. A pair or square with any block on floor or ice is held up, even with its other blocks over pits.
14. A fallen piece never moves again. It fills its pit: other pieces move onto it as onto floor.
15. Fallen girls stick like standing ones (two fallen pairs side by side make a fallen square).
21. A piece can start the level already fallen in a pit (a boy, a girl group). It never moves: the others come to it.

**Height**
16. A piece standing on a fallen piece touches it. A piece standing on floor beside a pit does not touch a piece that
    has fallen into that pit: they are at different heights. But a girl standing on a fallen girl of her colour does
    not stick to her: sticking is side by side, at the same height (rules 7, 26).
26. Pieces at the same height touch side by side: both standing, or both fallen. A boy who falls into a pit touches
    girls lying fallen in the pits beside him.

**Sliding**
23. A move goes one cell. If that cell is ice, the piece slides on, and keeps sliding while everything under it is
    ice. A single that reaches a pit falls in. A pair with one block over a pit and the other on ice is held up and
    slides on. A pair with any block on floor stops, and so does a piece that steps onto a fallen one.
24. A girl or pair sliding on ice stops where it sticks, even with free ice ahead.
27. A slide goes straight on, in the direction of the move. It never turns a corner.
28. A slide stops where a contact happens. A girl sliding past the boy meets him the moment she is beside him, and a
    boy sliding past a girl meets her the moment he is beside her: the slide stops there, and the contact happens.

**Cars**
19. A car is a piece moved like any other: one cell on floor, sliding on ice, falling into a pit like any piece.
20. A car never reacts: it doesn't stick, the boy doesn't clear it, and it need not go. A fallen car fills its pit
    and is floor from then on.

**Who reacts**
29. Only the moving piece reacts, where it stops: it sticks to girls already there and meets a boy already there,
    though they never moved. Pieces at rest never react, even when they touch from the start: four girls standing
    as a 2x2 block at the start are four singles until one of them moves.

**Craters**
30. A clear leaves pits (craters): every cell under the boy and the groups he cleared becomes a pit, except where a
    fallen car lies under them (it stays, and its cell stays filled). Later pieces can fall in, and a later boy can
    use the new pits.
    Cars never go in a clear (rule 20), and cells under nothing that went don't change; a boy who fell into a pit is
    gone after the clear, and his pit is empty again.

**Rare rules (lesson 17)**
31. A piece standing on a piece that is cleared falls into the pit left under it.
32. Cars move over fallen girls and fallen boys as over floor, with no reaction.
33. A girl who touches several boys at once clears all of them with her group.

**Damaged ground (Private Garden 2, lesson 18)**
34. Damaged ice and damaged floor wear as pieces pass over them. Cracked ice bears one more passing, then becomes
    shattered ice; shattered ice becomes a pit when a piece leaves it. Worn floor goes the same way, through rubble,
    to a pit.
    A cell wears each time a piece leaves it, also by sliding across it; the cell a piece stops on is not worn until
    it leaves.

**Balls (Private Garden 2, lesson 19)**
35. Balls (stone balls and ice balls) roll like a slide, until something stops them or they drop into a pit. A ball
    in a pit fills it: a stone ball with floor, an ice ball with ice (which later pieces slide over). A ball never
    reacts with girls or boys; a piece sliding into a ball stops beside it. Balls roll over fallen pieces like
    ground.

**Warps (Private Garden 2, lesson 20)**
36. Warps come in linked pairs. A one-block piece (a single girl, the boy, a car, a ball, a gay tile) entering one
    comes out of the other and goes on the same way. If the cell beyond the exit is taken, it comes out onto the exit
    and stops there, reacting or sticking with what is beside it. If the exit itself is taken, nothing goes through:
    a ball rolls on over the entry as over floor, any other piece stops on it. A single that would react or stick with
    something beside the entry does so there and never goes through. A pair crosses a warp as if it were floor. A
    warp destroyed by a clear is a pit, and its partner becomes plain floor.
    A warp is not damaged ground: it never wears.

**Gay tiles (Private Garden 2, lesson 21)**
37. Gay tiles (a man's face; the hints call them 兄貴, "big brother"): a gay tile and a boy that touch both vanish,
    and the ground under them becomes pits, also when the gay tile lies fallen in a pit. Two gay tiles that touch
    both vanish, leaving pits; one touching several at once takes them all. Gay tiles ignore girls and cars.
    A gay tile moves like any one-block piece, and its slide stops where it touches a boy or another gay tile.
    A girl lying fallen under a gay tile that vanishes stays there (gay tiles ignore girls).

## Rules not taught yet

**Private Garden 3** (not met yet)
38. Lesbian tiles: not met in any level yet. Their rules are unknown until a level with one is played.

## Habits that make solving work

1. **Read the cell list**, not the picture. Name the ground of every cell a piece passes.
2. **Plan backwards.** Before any move: where can the boy end (follow every route he has; slides often end in a pit)?
   Which cells does he touch there, and at what height? So where must every girl group be at that moment? Only then
   ask how the girls get there.
3. **Ask what each odd feature is for.** Levels are designed: alternating ice in two columns is a lane for a lying
   pair; a car next to a pit is a filler; a lone boy above an ice column is meant to slide down it.
4. **A pair's shape decides where it can go.** A lying pair spans two columns and can cross a lane where every row has
   one ice cell; an upright pair stays in one column and falls into the first two pits in it.
5. **Stoppers.** On open ice nothing stops by itself. To stop a piece on a cell, first park another piece just beyond
   it: a car, the boy, another girl. Every move changes which pieces can stop which.
6. **One contact per boy.** Two single girls can't arrive beside the boy one after the other: the first meets him
   alone. Join them into one group first, or bring them so that one move touches both.
7. **Keep the board as it stands.** After each move write "Now:" with where every moved piece is, and check the next
   move against that line, never against the starting position.
8. **Write each move as "piece, from-cell → to-cell (direction)"**, and check that the direction matches the numbers.
9. **Say "stuck at ..." and stop** when you are stuck. A guess dressed as an answer is worse than no answer.
10. **Answers only.** The reply holds the moves (one short line each) and the total; the working stays out of it.
11. **Check beside every cell of a slide.** At each cell a sliding piece passes, look at the four cells beside it:
    a girl there may stick (rule 24), a boy there makes the contact (rule 28). Either way the slide stops on that
    cell. Looking only along the row or column of the slide misses them (lessons 13, 18, 21, 23). Write the slide
    out: one short line per cell it reaches, with what is beside it, until it stops.
12. **A fallen piece is touched from on top.** A group standing on a fallen boy touches him (rule 16), and a boy
    standing on a fallen group touches it; standing beside it, a piece does not. So a boy down in a pit is reached by
    bringing a girl group onto his cell, often as the last move, sticking to another group as it arrives (rule 22).
13. **Who reacts with whom.** For each cell beside a slide's path, read in the cell list what stands there, then:
    - a moving girl beside a single girl of her colour: sticks (a pair); beside the boy: contact, both vanish;
      beside a gay tile: nothing (gay tiles ignore girls);
    - a moving boy beside a girl group: contact, both vanish (a boy never sticks); beside a gay tile: both vanish;
    - a moving gay tile beside the boy or another gay tile: both vanish; beside a girl: nothing;
    - a moving pair: sticks only to a pair that makes a 2x2 with it; a single beside it: nothing (rule 10);
    - a piece standing beside a fallen one: nothing (another height, rule 16).
    Each block of a moving group has its own neighbours: check them all.
