# [SkeletonGL](https://xenobyte.xyz/projects/?nav=skeletongl)

SkeletonGL is a 2D rendering engine written in C++ with a focus on performance and flexibility, it offers a feature-complete, ready to use template to immediately begin working on the essential components of the application without having to first write an underlying foundation.


The engine is written in multiplatform C++ and relies exclusively on free and open libraries to provide everything a GPU accelerated program needs to deliver on the harshest
standards. It's design abstracts away OpenGL's shortcoming by offering a dead simple interface to the engine's API together with an easily modifiable OpenGL 3.3+ wrapper that allows
for specialized builds and effective debugging techniques.


All modern OpenGL rendering capabilities are available, making it a more complete alternative to SDL's 2D renderer
while providing a very similar interface, its just as easy to use but with the added benefit of everything a core
graphics engine should. If you're looking for a complete, yet unobtrusive solution for graphical desktop development, SkeletonGL is for you.



**HEXmacs should work with any EMACS 25+ installation, but it is maintained for the newest stable release.**

## Dependencies

* [GLM](https://glm.g-truc.net/)
* [stb_image](https://github.com/nothings/stb/blob/master/stb_image.h)
* [freetype](https://www.freetype.org/)
* [SDL2](https://www.libsdl.org/index.php)
* [GLEW](http://glew.sourceforge.net/)

## Features

* Updated and ready for EMACS 27+
* Fully featured development environments and setups for C, C++, lua, python, javascript, LISP, bash, PHP and more
* Grammar & spelling correction suite for all available langauges (locale.gen)
* Organized template based on pure EMACS LISP (no package loading dependencies at all)
* Unobtrusive configuration that can be easily exapnded upon
* Automated package management
* Much smaller and faster than alternatives like spacemacs
* Regularly updated and kept at bleeding-edge state

## Installation

1. Install dependencies

    For Debia/Ubuntu systems:


    ```sh
    sudo apt-get update
    sudo apt-get install libsdl2-dev libglew-dev libfreetype6-dev
    ```

    For Arch based systems:

    ```sh
    sudo pacman -S sdl2 glew freetype2
    ```
    
2. Clone the SkeletonGL repo:

    ```sh
    git clone https://git.xenobyte.xyz/XENOBYTE/skeletongl
    cd skeletongl/
    make
    ./sgl
    ```

## Documentation

The source code is thoroughly documented using the doxygen standard, any doxygen generator can parse the code and output the API's specification into a portable format of your choosing.
The root folder contents are already setup as a template for new projects, simply add your own source code to the /src/ folder and update the makefile: 
  
Root project folder:


* src/: Source code folder
* static_lib: Compile the SGL insto a static (.a) library
* static_exe: Statically compile the sgl.a lib into the final executable
* makefile: Dynamically compile the final executable
* skeletongl.ini: Runtime settings file


**src/ code folder:**

* skeletongl/: SkeletonGL library source code
* skeletongl/skeletonGL.hpp: Monolithic include file
* skeletongl/window/: Window manager and main library interface
* skeletongl/renderer/: All render and OpenGL related code
* skeletongl/utility: Data structures, constants and general utility
* skeletongl/deps: Header only dependencies (GLM & stb_image)


Note that the entire SkeletonGL interface can be seen in the window/window.hpp file.
Visit the official project site at [xenobyte.xyz](https://xenobyte.xyz/projects/?nav=skeletongl) for more information.

## Example programs

The following programs are made in SkeletonGL and free for you to tinker with.

[snake-sgl](https://xenobyte.xyz/projects/?nav=snake-sgl) // Simple snake clone and first SkeletonGL example program

[cas-sgl](https://xenobyte.xyz/projects/?nav=cas-sgl) // Conway's game of life simulator made in SkeletonGL & C++ with a focus on performance.



