# OpenGL – Three Types of Triangles

## 📌 Project Overview
This OpenGL program displays **three different types of triangles** — a right-angled triangle, an equilateral triangle, and an isosceles triangle — on the screen.  
Each triangle is:
- **Positioned** in a different coordinate area of the viewport  
- **Colored** differently for easy distinction  
- Rendered using **GLFW** and **GLAD**  

---

## 🎯 Features
- **Right-Angled Triangle** in the **1st quadrant**  
- **Equilateral Triangle** in the **2nd quadrant**  
- **Isosceles Triangle** in the **3rd quadrant**  
- Three different colors (customizable)  
- Uses **modern OpenGL (GLSL shaders)**  

---

## 📂 File Structure
```
├── include/          # Header files
├── src/              # Source code files
│   ├── main.cpp      # Main OpenGL program
│   ├── glad.c        # GLAD loader
├── shaders/          # Vertex & Fragment shader files
├── build/            # Output executable
└── README.md         # Project documentation
```

---

## 🛠 Requirements
Make sure you have the following installed:
- **C++ Compiler** (GCC, MinGW, or MSVC)  
- **OpenGL** (version 3.3 or above)  
- **GLFW**  
- **GLAD**  

---

## 📥 Installation
1. Clone or download this repository:  
   ```bash
   git clone <repository_link>
   cd <repository_name>
   ```
2. Install dependencies:  
   - GLFW: [https://www.glfw.org/download.html](https://www.glfw.org/download.html)  
   - GLAD: [https://glad.dav1d.de/](https://glad.dav1d.de/)  

---

## ▶️ Running the Program
1. Compile the program (example for g++):  
   ```bash
   g++ src/main.cpp src/glad.c -Iinclude -Llib -lglfw3 -lopengl32 -lgdi32 -o build/main.exe
   ```
2. Run the program:  
   ```bash
   ./build/main.exe
   ```

---

## 🎨 Colors & Positions
| Triangle Type        | Quadrant  | Color (Default) |
|----------------------|-----------|-----------------|
| Right-Angled         | 1st       | Red             |
| Equilateral          | 2nd       | Green           |
| Isosceles            | 3rd       | Blue            |

---

## 📸 Output Preview
*(Example — Actual output will depend on your colors & positions)*  
```
    ▲   (Equilateral - Green)
   ▲▲
      (Right-Angled - Red)   (Isosceles - Blue)
```

---

## 📄 License
This project is for **educational purposes**. You may use and modify it freely for learning.
