# Play Tic Tac Toe
For this interactive section, we are going to play some games of Tic Tac Toe. You can try it anywhere, but there’s a really good one at this 
URL:[ https://playtictactoe.org/ ](https://playtictactoe.org/)

Think about what the computer is doing. If we know how to play the game already, we probably either win, or tie, but we’ll rarely lose, 
as it is such a simple game for us to beat the "AI" that we’re playing against. Play a few times, and think about what the computer is doing.
If we know how to play the game already, we’ll probably either win, or tie, but we’ll rarely lose, as it is such a simple game for us to 
beat the "AI" that we’re playing against.

## After playing tic-tac-toe a few times, try this
1. When it's our turn to go first, don't choose the center. For example, start at the top left corner. How does the computer respond?
  ..It doesn’t always go to the center as we might expect! (If it does, refresh the browser and try again.)
2. If it doesn't go to the center, place two Xs in a line on one of the edges on our next turn. Avoid the center yourself.
  ..The computer will block our three in a row because it has to.

The computer will go to the first available space on the board but it will learn from the board state that if that place led to a loss previously, 
then it won’t take it and will go to another available place instead. We’ll see over the first few games that we beat the computer easily. We
went as X, and the computer went as O.
The computer’s first move is to the top left corner.
Its second move is to the top center, and it loses frequently.
....**But then it learned how to avoid defeat in just a few games.**
_______________________________________________________
## Conclusion
So, from analyzing these (tic tac toe) moves, we can see that the computer has a rule to always block a three-in-a-row, but the programmers didn’t
consider the scenario that the center might be free, and didn’t program a rule to take the center if it is available! This teaches us that when we 
try to use rules for a scenario, it’s easy for us not to consider all cases, and to get it wrong as this game does!
