# Coin Collector Refactoring

[![Run on Repl.it](https://repl.it/badge/github/upperlinecode/coin-collector-refactor-javascript)](https://repl.it/github/upperlinecode/coin-collector-refactor-javascript)

## What We're Building

Last week, we made a simple game where a player moved their mouse around the screen to collect as many coins as possible before time ran out. This was great, but now that's we have experience with classes, we can make it even better.

We have two reasons for refactoring the code with classes:
1. It's great practice with using classes, and
2. It will allow you to super easily add multiple coins to the screen, which will make the game more interesting.

## The Approach

If you or your partner can find your code from last week, copying it into a new project is a great way to begin. If you're having trouble locating it, you can find approximately what we wrote together in the file `starter.js`.

It is going to be the job of you and your partner to figure out the specific steps needed to refactor this code, but here is a basic outline of how you might go about it.

Start by creating a `Coin` class. It's going to need a constructor which takes `x` and `y` as parameters. What's it going to do with them?

Now add a `display` method which draws the coin to the canvas.

Then add a longer method called `checkCollection` which checks if the user's mouse has come close enough to collect the coin. If so, it should move itself to a random position and increment score.

Let's start with just one coin. Let the variable you already have (called `coin`) be initialized to an instance of this new class. Then in the `draw` loop, you're going to need to tell this coin to `display` itself and to `checkHit`. Make sure to remove any extraneous code relating to the old method.

### Stretch

Once this is working to your satisfaction, and if you have time, go ahead and try to have two or three coins on the screen at once, using an array. You'll want a new  variable called `coins` which starts with a couple coins in it. Then loop over them to `display` and `checkHit` in your `draw` loop.
