# jsSud
a Javascript Sudoku Game

So, here is the basic idea.
Write a game of Sudoku.

the concept is to keep as much as possible to me to the basic principles of OOP.

cell/tile is a numberContainer.
each number is container.
there should be a group of cells
 - 3x3 - 9 times
 - 1x9 - 9 times
 - 9x1 - 9 times

each sigle cell should have 9 numberContainers for the hints storing.

each cell when sellected will:
 - pop zoomed-in the 9 smaller numberContainers.
 - each of them
 	- when tapped will toggle active/inactive state.
 	- when pressed for a little longer time will be selected as a chosen number and will zoomout
 	- when touch is outside: will zoomout the view and leave the view.

each group when completed will be highlight:
 - with different colors will be highlighted the 3 different kind of groups. 

when all groups are done:
 - game will splash a nice "Congratulations!" splash



 For the Solver:
  - has to be researched for a good solution finder algorithm
  - has to be considered a variational statistic algorithm 
  - to be able to use hints (probably in the full/payed ;) version if I decide to make it paid)
  - to have the function to enter a paper-read-sudoku and solve it.

For the generator:
  - to be considered a permutational/variational related algorythm
  - to be considered a uniqueness of the solution

For the general idea:
 - have a leader board
 - login with facebook/gmail or something else.
 - django-social can be used for this purpose.
 - there is an already suitable library for the purpose: django-leaderboard