# Clear Colored Window (OpenGL + GLFW + GLAD)

This project is a basic OpenGL application that creates a window using **GLFW**, loads OpenGL functions using **GLAD**, and clears the window with a **cyan background color**.  
The program also demonstrates keyboard input handling and window resizing.

---

## 🛠 Technologies Used

- **C++**
- **OpenGL (Core Profile 3.3)**
- **GLFW** – window creation and input handling
- **GLAD** – OpenGL function loader
- **MinGW (Windows)** / **GCC (Linux)**

---

## 📂 Project Structure

```

HelloWindowClearColored/
│
├── include/
│   ├── glad/
│   │   └── glad.h
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

## 🚀 Features

- Creates an **800 × 600** OpenGL window
- Clears the screen with **cyan color**
- Window title set to **"Sadia Jannat"**
- Press **`S` key** to close the window
- Automatically adjusts viewport on window resize

---

## 🧪 Build & Run Instructions

### 🔹 Windows (MinGW)

#### Requirements
- MinGW installed
- `mingw32-make` available
- `libglfw3.a` in `lib/`
- `glfw3.dll` placed in `build/` (or same directory as `main.exe`)

#### Build & Run
```powershell
mingw32-make win
````

This will:

* Compile the program
* Generate `build/main.exe`
* Run the executable

---

### 🔹 Linux

#### Requirements

* GCC
* GLFW development package
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

## 📘 Notes

* GLAD is initialized using `glfwGetProcAddress`
* The program uses **OpenGL Core Profile 3.3**
* Framebuffer resize callback ensures correct viewport scaling

---

## 👩‍💻 Author

**Sadia Jannat**

---

## 📜 License

This project is for **educational purposes only**.

```
