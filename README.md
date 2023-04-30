# Cube-RGB

<p align="center">
  <img style="text-align: center;" height="250px" src="./Images/Result.png" alt="Alt text">
</p>

## Introduction

This repository contains an RGB cube designed with OpenGL, C++ and CMake

## How it works?

Each Vertex of this cube has a unique combination of 0s and 1s that form the colors of the cube.

<img height="200px" src="./Images/Cores.png" alt="Cores">


## How to Execute?

First check if the dependencies are installed

```bash
sudo nala install libglfw3-dev libglm-dev libglew-dev libstb-dev libglm-doc
```

Generate the Makefile

```cmake
cmake -H. -BBuild -DCMAKE_RUNTIME_OUTPUT_DIRECTORY=./Bin
```

- `-H.` Look for CMakeLists.txt in the current directory
- `-BBuild` Paste the generated Makefile inside the Build folder
- `-DCMAKE_RUNTIME_OUTPUT_DIRECTORY=./Bin` Adds the final executable to the ./Build./Bin folder

Finally, compile and run the program.

```make
make -C ./Build && ./Build/Bin/Cube-RBG
```