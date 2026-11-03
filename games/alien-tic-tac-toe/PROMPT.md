# Alien Tic-Tac-Toe

Build a browser game: Alien Tic-Tac-Toe.
Recipe: Alien Tic-Tac-Toe (featured class example).
One round: start → play → result → restart.

## Brief

- Title and theme: Alien Tic-Tac-Toe — solo board + short alien battles
- Player goal: Get three X marks in a row, column, or diagonal
- Main action: Click an empty square, then pick Shield / Blast / Dodge
- How a round ends: X line (you win), O line (aliens win), or full board with no line (draw)
- Round length: Nine battles at most; each battle is 2–3 exchanges
- Out of scope: Timers, sound, logins, random alien moves, extra art packs

One-sentence game: The player fights for each square to earn X marks before the aliens complete a line of O.

## Rules

This is a solo three-by-three board. You choose every square. A short battle determines who receives it.

1. Start with an empty board.
2. Select an empty cell. That cell becomes the pending battle location and the whole board locks.
3. Win the battle to put **X** in the selected cell. Lose the battle to put **O** there.
4. There is no automatic opponent move. One finished battle fills exactly one cell.
5. Three X marks in any row, column, or diagonal wins the board. Three O marks loses it. A full board with neither line is a draw.
6. If the board is not finished, return to it and choose another empty cell.
7. **Restart game** abandons the whole board immediately, including any battle in progress.

## Battle

Every battle starts with 2 player health and 2 alien health. Show health as text: “You: 2 of 2” and “Alien: 2 of 2”.

The alien announces its move. You choose one of three responses:

| Alien shows | Correct response | Result if correct |
| --- | --- | --- |
| Laser | Shield | Alien loses 1 health |
| Shield | Blast | Alien loses 1 health |
| Claw | Dodge | Alien loses 1 health |

Any other response costs the player 1 health. Exactly one side loses exactly one point per accepted response.

First version sequence: Laser → Shield → Claw, restarting at Laser for every new battle. Correct answers: Shield → Blast → Dodge.

After a response, disable all response buttons and show what happened. If both sides still have health, show **Next exchange**. If the alien reaches zero health, the battle ends with a win. If the player reaches zero, it ends with a loss.

Win / lose / draw must be visible on screen.
No login, no server, no leaderboard.
Single HTML/CSS/JS page is fine.
After a round, Play again must reset all round state.
