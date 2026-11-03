# Flappy Bird

Build a browser game: Flappy Bird.
Recipe: one-button tap-to-flap (from the space dodger).
One round: start → play → result → restart.
Main control: tap, click, or Space to flap.

## Brief

- A small bird falls unless the player taps a visible Flap control, taps the playfield, or presses Space
- Each press is one flap. Holding does not keep the bird up
- Green pipes approach with a gap. Passing one pipe earns one point, once
- A visible collision with a pipe or the ground ends the round and shows the score and Play again
- The top of the sky stops the bird; only pipes and the ground end the round
- The first flap starts the round from a waiting pose
- Replay resets bird position, pipes, score, and movement
- Instructions hold the game idle before Start
- No login, no server, no leaderboard
- Single HTML/CSS/JS page is fine
- After a round, Play again must reset all round state
