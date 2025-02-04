# Sys-Mon (System Monitor in C++)

![System Monitor](images/system-monitor.jpg)

## ncurses
[ncurses](https://www.gnu.org/software/ncurses/) is a library that facilitates text-based graphical output in the terminal. This project relies on ncurses for display output.

Install ncurses within your own Linux environment: `sudo apt install libncurses5-dev libncursesw5-dev`

## Make
This project uses [Make](https://www.gnu.org/software/make/). The Makefile has four targets:
* `build` compiles the source code and generates an executable
* `format` applies [ClangFormat](https://clang.llvm.org/docs/ClangFormat.html) to style the source code
* `debug` compiles the source code and generates an executable, including debugging symbols
* `clean` deletes the `build/` directory, including all of the build artifacts

## Instructions

1. Clone the project repository: `git clone git@github.com:l0g1c-80m8/system-monitor.git`

2. Install cmake `sudo apt-get -y install cmake` and ncurses 'sudo apt install libncurses5-dev libncursesw5-dev'

2. Build the project: `make build`

3. Run the resulting executable: `./build/monitor`

## Tasks

- [x] Calculate CPU utilization dynamically, based on recent utilization
- [ ] Make the display interactive to sort processes based on CPU or memory utilization
- [ ] Refactor the project to use abstract classes (interfaces) and pure virtual functions
- [ ] Port the program to another operating system
