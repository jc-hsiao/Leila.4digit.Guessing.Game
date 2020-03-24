# The Classic 4-digit number guessing game

At the start, the game secretly generates a four-digit unique number-set for the user to guess.
The player can play by continuously entering four-digit number, 
The game will print out messages to the player every time they guess.

##Generate
- The numbers in the four-digit number set should be unique, it can be 1934, 5968...etc, it should not generate 1229, 8834...etc
- The four-digit number set should be able to have 0 as the first digit. So if you are only generating random number from 1000 to 9999, then you are doing it wrong! The game should be capable of generating 0123, 0987 and so on.

##Game Response
- If the number-set given by the player has a number that matches the answer, but the position of the number does not match. The game will count 1B. And if there are more, it will print 2B, 3B or 4B.
- If the number-set given by the player has a number that matches the answer, and the position of the number also matches. The game will count 1A. And if there are more, it will print 2A, 3A or 4A.
- Some example to make things more clear:
  - if the answer is 5678 and user guessed 1234, it should print 0A0B 
  - if the answer is 5678 and user guessed 4567, it should print 0A3B
  - if the answer is 5678 and user guessed 5789, it should print 1A2B
  - if the answer is 5678 and user guessed 5679, it should print 3A0B
- If the player guessed the number-set with exact numbers and position, which is 4A0B, player wins the game.

