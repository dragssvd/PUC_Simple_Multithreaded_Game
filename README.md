# PUC-Simple-Multithreaded-Game
University assignment for Operating Systems course.
Written in pure C language using pthreads, semaphors and ncourses.

## Multithreading Implementation:

The game employs multithreading to manage concurrent player actions and game events. Each player and beast operates in its own thread, allowing for simultaneous movements and interactions. This design ensures that the game remains responsive, with the server efficiently handling multiple threads corresponding to active players and beasts.​

## Server-Client Architecture:

The server maintains the global game state, including the positions of players, beasts, coins, and other game elements. Players connect to the server as clients, receiving updates about their immediate surroundings and sending their actions back to the server. This architecture centralizes game logic on the server side, reducing the computational load on individual clients and ensuring consistency in the game state.

## Server view:
![image](https://user-images.githubusercontent.com/97313850/203628411-0a8a34f2-9972-4d26-9486-4f6d8015b53a.png)

c - coin

C - 10 coins

T - 50 coins

D - coins dropped by players

1-4 - Players

'*' - Beasts add as many as you want

A - campsite

'#' - brushes which slow your movement

## Player view:

![image](https://user-images.githubusercontent.com/97313850/203628498-97869b28-9cce-4b6e-91a7-2fba4feae655.png)

Player is shown just his stats, position and closest surroundings inlcuding other players or monsters.

Contains some fancy makefiles for ease of use.
