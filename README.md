# C++/OpenGL 3D-Object API
A basic C++/OpenGL 3D-Object API. Originally intended for use as part of a 3D visualization tool for another project.

This API is in *rough form* as it was built for both a very specific purpose for a senior project as well as an exercise in learning OpenGL.

## Dependencies
__\* The code has only been tested on Ubuntu 16 & 17 Linux system. A Debian Linux distribution is recommended. \*__
- CMake
- GCC compiler
- OpenGL
- freeGlut
- GLM (Graphics Language Mathematics)

## Installation & Demonstration
Once you have the necessary libraries, you can use CMake to build the debugger tool to view a demonstration of the code in action.

In shell/command-line, change working directory to the reposirtory directory and run the cmake script:
```
cmake CMakeLists.txt
```
Build the target in the current directory with:
```
cmake --build .
```
Run the demonstration:
```
./opengl-debugger
```
