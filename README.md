# The Maze

The Maze is a three-dimensional game developed using SDL2 and Raycasting. Players can navigate in all four directions on the map using the keys `W`, `A`, `S`, and `D`.

Moving through the maze, players have the freedom to turn left or right as they please.

In the event of a collision with a wall, players cannot proceed unless they change their direction.

Players are capable of moving in various directions and simultaneously rotating.

## Installation

Clone this repository:
```bash
git clone https://github.com/johnechono/The-Maze.git
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
- `N` - Turn on map visibility. The 2D map will be visible again if it wasn't

***Enjoy your gaming experience!***

# Directories

[`src`](https://github.com/johnechono/The-Maze/tree/main/src) - Encompasses all the source code files written in C.

[`inc`](https://github.com/johnechono/The-Maze/tree/main/inc) - Houses all the header files.

[`maps`](https://github.com/johnechono/The-Maze/tree/main/maps) - Stores map data files, which the program utilizes to output the map layout.

[`images`]() - Contains image files.

# Images

![image](https://user-images.githubusercontent.com/44834632/138765500-bd3838d0-fe46-4018-87b0-21143fb77e8b.png)

## Texture sources

**Weapon**

[Source](https://www.seekpng.com/idown/u2w7u2t4i1y3a9y3_call-of-duty-guns-firearms-gun-weapons-coat/)

## Contributing

- Familiarize yourself with the source files in the `src` folder and the header files in the `inc` folder.
- Clone the repository and create a new branch: `$ git checkout https://github.com/johnechono/The-Maze -b [name_of_new_branch]`.
- Introduce a feature, rectify a bug, or refactor some code :)
- Draft or update tests for the changes made, if needed.
- Modify `README.md` as necessary.
- Initiate a Pull Request accompanied by a comprehensive description of the changes.

# Author

Echono John Inalegwu ([GitHub](https://github.com/johnechono))
