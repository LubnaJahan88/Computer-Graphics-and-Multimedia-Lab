# 🧊 Cyan Square with Triangle - OpenGL Project

## 🎯 Project Description

This OpenGL project displays a **cyan-colored square** on a **white background**, with a **cyan triangle** sitting on top of the square. The triangle shares the top two corner points of the square, forming a simple but visually meaningful composition.

The window title is set to **"Lubna Jahan"**, and the program automatically closes when the **`L` key** (first letter of the name) is pressed.

## 🖼️ Output Preview

- ✅ Cyan square rendered at center
- ✅ Cyan triangle rendered above square
- ✅ White background
- ✅ Window closes when `L` is pressed

## 💻 Tech Stack

- **C++**
- **OpenGL 3.3**
- **GLFW**
- **GLAD**

## 📁 Folder Structure

```
project-root/
│
├── include/           # Header files (e.g., glad.h, glfw3.h)
├── src/               # Source files (e.g., main.cpp, glad.c)
├── build/             # Compiled output
├── lib/               # Precompiled OpenGL libraries (e.g., glfw3.lib)
├── README.md          # This file
├── CMakeLists.txt     # Optional: for build automation (if using CMake)
└── Makefile           # Optional: for manual compilation (make)
```

## ⚙️ How to Build & Run

1. **Install Dependencies:**
   - [GLFW](https://www.glfw.org/)
   - [GLAD](https://glad.dav1d.de/)
   - OpenGL (already available on most systems)

2. **Build using `g++`:**

   ```bash
   g++ -Iinclude src/main.cpp src/glad.c -o build/main.exe -Llib -lglfw3 -lopengl32 -lgdi32
   ```

3. **Run the executable:**

   ```bash
   ./build/main.exe
   ```

## 🧪 Features Implemented

- [x] Cyan square using two triangles
- [x] Cyan triangle on top sharing corner points
- [x] White background
- [x] Close window on key press (`L`)
- [x] Clean shader setup (vertex + fragment)
- [x] Proper VAO and VBO setup

## 🎓 Learning Outcomes

- Setting up an OpenGL environment using GLFW and GLAD
- Using vertex buffer objects (VBO) and vertex array objects (VAO)
- Writing custom vertex and fragment shaders
- Drawing multiple shapes
- Handling keyboard input events in OpenGL

## 🙋‍♂️ Author

**Lubna Jahan Lipa**

## 📝 License

This project is for educational purposes only. You are free to fork, modify, and use it with attribution.