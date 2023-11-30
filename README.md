# The Maze

The Maze is a three-dimensional game developed using SDL2 and Raycasting. Players can navigate in all four directions on the map using the keys `W`, `A`, `S`, and `D`.

Moving through the maze, players have the freedom to turn left or right as they please.

In the event of a collision with a wall, players cannot proceed unless they change their direction.

Players are capable of moving in various directions and simultaneously rotating.

## Installation

Clone this repository:
```bash
git clone https://github.com/johnechono/Maze-Game.git
```

## Compiling

This project relies on gcc and make for the compilation process.

### Windows

Ensure gcc and make are installed, preferably through chocolatey. Then execute the following command:
```bash 
make
```

### Linux

Ensure SDL2 is installed. If not, run the following make commands: 
```bash
make linux_install
```
Then compile using:
```bash
gcc src/*.c -Wall -Werror -Wextra -pedantic -lSDL2 -DLINUX -o maze -lm
```

### Mac

Ensure SDL2 is installed, then run the following command:
```bash
make mac
```

## Running

After a successful compilation, run the program using the following command:
```bash
./maze MAP
```
Here, `MAP` is the name of the file found in the maps folder. Additional maps can be created and passed while running the program as described above. Map files only accept the allowed characters.

## Controls

- `W` - Move forward
- `S` - Move backward
- `A` - Look left
- `D` - Look right
- Mouse move left/right - Look left or right
- `M` - Turn off map visibility. The 2D map won't be visible on clicking
- `N` - Turn on map visibility. The 2D map will be visible again

# Author

Echono John Inalegwu ([GitHub](https://github.com/johnechono))
