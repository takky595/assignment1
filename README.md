# CSI281 Assignment 1

This assignment will act as a review of C++ concepts from CSI 140 and 240. At the top of each file is a note about whether or not you should modify it. Please only modify the files that are indicated as being okay to modify.

The goal of this assignment is to read a `.csv` file containing temperature data about NYC and Burlington into structs/classes, process it, and draw some charts of it.

## Basic Instructions

1. Download the contents of this repository.
2. Create your own private repository and add the contents of this repository to it.
3. Add your partner and me (@davecom) as collaborators on your private repository.
4. Implement the missing parts where it says "YOUR CODE HERE"
5. Test it by following the build directions below.
6. Submit the URL to your private repository on Canvas.

## Directory Structure and Files

- `/` Main directory including this `README.md`, the build scripts, and the `.csv` file.
- `/lib` Libraries for drawing the charts and testing your work. There's no need to touch this.
- `/src` Source files, some of which you should modify and some of which you should not.

### Specific Files

*indicates do not modify
&indicates you must modify

- `GNUMakefile`* make file for GNU Make on macOS and GNU/Linux
- `Makefile`* make file for nmake/Visual Studio on Windows
- `README.md`* this file
- `LICENSE` MIT License
- `tempdata.csv`* temperature data about NYC and Burlington. You can open this in a text editor or Excel if you want to browse it.

- `lib/catch.h`* a unit testing library
- `lib/PPlot.cpp`* part of a chart making library
- `lib/PPlot.h`* part of a chart making library
- `lib/SVGPainter.cpp`* part of a chart making library
- `lib/SVGPainter.h`* part of a chart making library

- `src/CityTemperaturedata.h`* defines a structure and a class for holding data
- `src/CityTemperatureData.cpp`& implementation of the class
- `src/csv.h`* function definitions for reading the CSV and turning it into CityTemperatureData
- `src/csv.cpp`& implementations of the above
- `src/main.cpp` the main file that runs the tests and makes the charts
- `src/test.cpp`* the unit tests to prove your code works

## Building and Running

### macOS and GNU/Linux

Run `make` and `./assignment1` to run all of the tests. It will also output two `.svg` files when you are done that show the data nicely plotted. Run `make clean` to remove all objects files, the executable, and the svg files.

### Windows

From the start menu (assuming you have installed Visual Studio 2019) open the "Developer Command Prompt." CD to the appropriate directory and run `nmake` and `assignment1` to run all of the tests. It will also output two `.svg` files when you are done that show the data nicely plotted. Run `nmake clean` to remove all objects files, the executable, and the svg files.
