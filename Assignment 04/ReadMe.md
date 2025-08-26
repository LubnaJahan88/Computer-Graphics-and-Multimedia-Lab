# OpenGL Dynamic Triangle Color

## Description

This is a simple OpenGL project built using C++ with GLFW and GLAD. The application displays an upside-down triangle centered on a black background. The triangle transitions its color dynamically between **cyan** and **white** over time, giving a smooth visual effect.

The window title is set to a student ID as specified: `0432310005101088`.

## Features

- Uses modern OpenGL (version 3.3 core profile)
- Dynamic color transition from cyan to white and back
- Responsive to window resizing
- Exits cleanly when pressing `ESC`

## Screenshots

![Triangle Preview](screenshot.png)

> _Add a screenshot to show the output (optional)._

## Dependencies

Ensure the following libraries are set up in your project:

- [GLFW](https://www.glfw.org/) (for windowing and input)
- [GLAD](https://glad.dav1d.de/) (for managing OpenGL function pointers)
- OpenGL 3.3 capable GPU and driver

## Build Instructions

### Prerequisites

- C++ Compiler (supporting C++11 or later)
- CMake (recommended) or manual Makefile
- GLFW and GLAD set up in your include and link paths

### Using CMake

```bash
mkdir build
cd build
cmake ..
make
./OpenGLDynamicTriangle
Replace OpenGLDynamicTriangle with your actual executable name if different.

Manual Compilation (Linux/macOS)
bash
Copy code
g++ main.cpp -o OpenGLDynamicTriangle -lglfw -ldl -lGL
Ensure glad.c is compiled and linked if you're using the GLAD C source file.

How It Works
The triangle is rendered using a vertex shader and a fragment shader.

The glUniform4f function updates the fragment shader's ourColor uniform every frame.

The red component of the color changes with sin(time), resulting in a smooth transition.

The triangle remains upside-down and centered regardless of window resizing.

Controls
Key	Action
ESC	Exit the application

Project Structure
makefile
Copy code
.
├── main.cpp
├── CMakeLists.txt       # If using CMake
├── README.md
└── (glad/, include/, lib/, etc.)  # Your dependencies
License
MIT License (or specify your own)

Author
Dr. Islam – Educational OpenGL demo
Student ID: 0432310005101088