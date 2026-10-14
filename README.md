# Projects

## maze-game
A 2D Pac-Man style maze game in C using [Simple 2D](https://www.simple2d.org/).

**Goal:** eat all the dots without touching the two enemies.
**Controls:** W / A / S / D

### Build and run
Install Simple 2D first, then from inside `maze-game/`:

```
simple2d build game.c
./game
```

Or with gcc:

```
gcc game.c -o game $(simple2d --libs)
./game
```

Run it from inside `maze-game/` so it can find `game.txt` and `vera.ttf`.
Sounds are optional: put `Game-Win-Sound.wav` and `Game-Loss-Sound.wav` in `Assets/`.

### Custom maze
Edit `game.txt`: `#` = wall, `.` = dot, space = empty floor.

## pdc-producer-consumer
Producer-consumer demo with threads, a mutex and a condition variable (C++11).

```
g++ -std=c++11 -pthread PDC1.cpp -o PDC1
./PDC1
```
