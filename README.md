# tictactoe
A Tic-Tac-Toe Game Written in Javascript

This tic-tac-toe game comes with 2 modes
1. Against a bot
2. Against another player

The bot is coded such that it plays somewhat optimally, any games played against it either end in a tie or a loss.

## Strategy of Bot
1. If a circle can be played such that the bot wins, the bot places the circle to win.
2. If the player can win in 1 turn, the bot plays to stop it
4. Edge Case: If the board is as follows (or 90 degrees rotation of the following), do the following move
<pre>
X| |               X|O| 
-----              -----
 |O|          -->   |O| 
-----              -----
 | |X               | |X
</pre> 
3. Else, try to play the center, if that is unavailable, play the corner, else play a random side.
