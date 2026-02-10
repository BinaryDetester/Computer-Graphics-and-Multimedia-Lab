# OpenGL Shader-Based Triangle Rendering (GLFW + GLAD)

This project demonstrates **modern OpenGL (Core Profile 3.3)** using **GLFW** and **GLAD**.  
It creates an OpenGL window, compiles and links **vertex and fragment shaders**, and renders **two triangles** using **VBO** and **VAO**.

The program also handles keyboard input and window resizing.

---

## 🛠 Technologies Used

- **C++**
- **OpenGL 3.3 (Core Profile)**
- **GLFW** – window creation & input handling
- **GLAD** – OpenGL function loader
- **MinGW (Windows)** / **GCC (Linux)**

---

## 📂 Project Structure

```

HelloWindowClearColored/
│
├── include/
│   ├── glad.h
│
├── src/
│   ├── main.cpp
│   └── glad.c
│
├── lib/
│   ├── libglfw3.a
│   └── glfw3.dll
│
├── build/
│
├── Makefile
└── README.md

````

---

## ✨ Program Features

- Creates an **800 × 600** OpenGL window
- Uses **custom vertex and fragment shaders**
- Renders **two triangles** using `glDrawArrays`
- Background color: **Orange**
- Triangle color: **Cyan**
- Uses **VBO (Vertex Buffer Object)** and **VAO (Vertex Array Object)**
- Press **`S` key** to close the window
- Automatically resizes viewport when window size changes

---

## 🎨 Rendering Details

### Vertex Shader
- Accepts vertex position (`vec3`)
- Converts it to clip-space using `gl_Position`

### Fragment Shader
- Outputs a solid **cyan** color using `FragColor`

### Geometry
- Total vertices: **6**
- Primitive type: **GL_TRIANGLES**
- Two triangles drawn in a single draw call

---

## 🚀 Build & Run Instructions

### 🔹 Windows (MinGW)

#### Requirements
- MinGW installed
- `mingw32-make`
- `libglfw3.a` inside `lib/`
- `glfw3.dll` placed in `build/` (or same folder as `main.exe`)

#### Build & Run
```powershell
mingw32-make win
````

---

### 🔹 Linux

#### Requirements

* GCC
* GLFW development libraries
* OpenGL libraries

#### Build & Run

```bash
make linux
```

---

## ⌨ Controls

| Key   | Action           |
| ----- | ---------------- |
| **S** | Close the window |

---

## 🖥 System Graphics Check

To verify OpenGL support:

### Windows

* Press **Win + R** → type `dxdiag`
* Check the **Display** tab
  OR
* Use **GPU-Z** to see OpenGL version

### Linux / macOS

```bash
glxinfo | grep "OpenGL renderer"
```

---

## 🧪 Student Tasks (Lab Work)

1. Draw an **upside-down green triangle** on a **black background**
2. Draw a **right-angle magenta triangle** on a **white background**

---

## 👩‍💻 Author

**Sadia Jannat**

**0432320005101108**


Computer Graphics & Multimedia Lab

---

## 📜 License

This project is intended for **academic and educational purposes only**.

```

