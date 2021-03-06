tennis_exercise
===========

French Open is hosting a tennis tournament. To aid with this, we're developing a scoring system.

The scoring system for tennis works like this.

A game is won by the first player to have won at least four points in total and at least two points more than the opponent.

The running score of each game is described in a manner peculiar to tennis: scores from zero to three points are described as 0, 15, 30, 40, respectively

If at least three points have been scored by each player, and the scores are equal, the score is "deuce".

If at least three points have been scored by each side and a player has one more point than his opponent, the score of the game is "advantage" for the player in the lead.

Constraints

We're just worried about one game, don't worry about sets, tie breakers, etc
Don't worry about validation, assume the client passes in correct data
For example:

The interface will look something like this in Java:


  Game game = new Game("player 1", "player 2");
  game.pointWonBy("player 1");
  game.pointWonBy("player 2");
  // this will return "15-15"
  game.score();

  game.pointWonBy("player 1");
  game.pointWonBy("player 1");
  // this will return "40-15"
  game.score();

  game.pointWonBy("player 2");
  game.pointWonBy("player 2");
  // this will return "Deuce"
  game.score();

  game.pointWonBy("player 1");
  // this will return "Advantage player 1"
  game.score();

  game.pointWonBy("player 1");
  // this will return "Player 1 wins"
  game.score();
Notes on implementation:

use Java, Javascript, Groovy, Scala, Ruby or C#
try not to spend more than 2 hours maximum. (We don't want you to lose a weekend over this!)
don't build guis etc, we're more interested in your approach to solving the given task, not how shiny it looks.
don't use any frameworks (rails, spring etc), or any external jars/gems (unless it's for testing..)

