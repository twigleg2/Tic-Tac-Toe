# Tic-Tac-Toe
Learn React by making a Tic-Tac-Toe game\
https://reactjs.org/tutorial/tutorial.html

## Why Immutability Is Important
### Complex Features Become Simple
Immutability makes complex features much easier to implement. Later in this tutorial, we will implement a “time travel” feature that allows us to review the tic-tac-toe game’s history and “jump back” to previous moves. This functionality isn’t specific to games — an ability to undo and redo certain actions is a common requirement in applications. Avoiding direct data mutation lets us keep previous versions of the game’s history intact, and reuse them later.

### Detecting Changes
Detecting changes in mutable objects is difficult because they are modified directly. This detection requires the mutable object to be compared to previous copies of itself and the entire object tree to be traversed.

Detecting changes in immutable objects is considerably easier. If the immutable object that is being referenced is different than the previous one, then the object has changed.

### Determining When to Re-Render in React
The main benefit of immutability is that it helps you build pure components in React. Immutable data can easily determine if changes have been made which helps to determine when a component requires re-rendering.