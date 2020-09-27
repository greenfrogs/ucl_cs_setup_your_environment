# The C Programming Language
> C has the power of assembly language and the convenience of … assembly language. -- *Dennis Ritchie*

Mac already has gcc and debugging tools installed for C so we just need to setup the IDE.

1. Open the Jetbrains Toolbox and install [CLion](https://www.jetbrains.com/clion/)

2. Press `New Project`, select C executable from the new project screen with any language standard.
A simple Hello World program should open and if you click the play symbol at the top right it will compile and execute
in a terminal at the bottom of the screen.

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}

```

## Additional Notes
1. CLion uses CMake to configure running your project. While others are worrying about linking new files to their project
you can simply add it to the `add_executable` section (as shown with `new_file.c` below).

```c
cmake_minimum_required(VERSION 3.16)
project(untitled C)

set(CMAKE_C_STANDARD 99)

add_executable(untitled main.c new_file.c)
```

2. If you ever need to pipe something from C to another program (such as a turtle program) then you can compile your
application with CLion (hammer icon) and then run your program in terminal with a pipe operator.

```bash
> .\your_program | turtle
```

3. If you ever need to access `gcc` directly then you can access it via your terminal.
