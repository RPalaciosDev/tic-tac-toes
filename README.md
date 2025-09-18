# Noughts and Crosses and Negamax

## Intro

This was the second major assignment for Advanced Game Development. We developed a two-person game of Noughts and Crosses. We later added a Negamax algorithm to serve as our Enemy AI.

### Setup

We were given fairly clear instructions on how to proceed in this project from our professor. As such, we mainly needed to read the comments and TODOs and implement them. Often this meant that we were stringing together premade functions or some of our own functions.

Of the functions we were tasked to complete, we had some freedom in `setUpBoard()`, `checkForWinner()`, and the state string functions. I had some difficulty deciding how to pass the vector to `initHolder()`. I ended up passing an anonymous vector with hardcoded size values to that function. While that works, I feel like there must be a better way to send that same information without hardcoding the values. As it stands, this solution is difficult to scale.

In `checkForWinner()`, we had to decide how to best check our winning triples. I ended up looking at each square in the triple, saving the pointer to the player-owner of the square and then checking the players at each location for equivalency. While this works, our professor later showed us a better implementation that doesn't save pointers for this purpose.

Lastly, the state string functions allowed us to work on our string building skills. I opted to use a stream for this purpose. Once again, our professor showed us a separate implementation that builds the string using much cleaner logic.

### Negamax

The previous work was done by me. The negamax algorithm, however, was given to us in class. All the students needed to do was follow along. While I got this to work, I do feel as though I need to look over the code further to fully understand it.
