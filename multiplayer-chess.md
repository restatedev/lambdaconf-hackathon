# Multiplayer chess game

In this scenario you will build a multiplayer chess game, like [Lichess](https://lichess.org/), using Restate.

Users join a waiting room, where the matchmaking system pairs two users, and afterward the game starts.

Some ideas to spice up your project:

* If you implement the coordinate system using UCI notation or FEN, you can easily visualize the board with real UIs like [this one](https://www.mathsisfun.com/games/chess.html) or [this one](http://www.ee.unb.ca/cgi-bin/tervo/fen.pl) or even build a UI yourself with [chessboardjs](https://chessboardjs.com/).
* The matchmaking can be as complex as you want, for example adding a ranking system.
* You could allow a player to "take over" the match of another player, in case one player is AFK for too long. 
* You can implement the CPU player by connecting to an existing game engine like [Stockfish](https://disservin.github.io/stockfish-docs/stockfish-wiki/UCI-&-Commands.html).
* If you don't like chess, any other online turn based game can work too, such as checkers, backgammon, naval battle, or any card game.