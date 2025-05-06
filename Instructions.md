

# *SETUP AND CONTROL INSTRUCTONS*!
  

### **Prerequisites:**  
- Ensure you have a C++ compiler installed (**GCC/MinGW** for Windows, **Clang/GCC** for Linux/macOS).  
- Install **OpenGL** and **GLUT** libraries.  

#### **Windows:**  
- Download and install **FreeGLUT**.  

#### **Linux/macOS:**  
Use the package manager:  
```sh
sudo apt-get install freeglut3-dev   # Ubuntu/Debian
brew install freeglut               # macOS
```  

### **Compilation and Execution (Without Code::Blocks)**  

Navigate to the project directory:  
```sh
cd YourProject
```  

Compile the program:  
```sh
g++ -o project main.cpp -lglut -lGLU -lGL
```  

Run the program:  
```sh
./project
```  

### **Running in Code::Blocks**  
1. Open **Code::Blocks**.  
2. Click on **File > Open...**, then select `main.cpp`.  
3. Ensure that you have set up a new project (or use an existing one) and added `main.cpp` to the project files.  
4. Click **Build > Build and Run**, or simply press **F9** to compile and run the program.  
5. If any errors occur, check if the **GLUT** and **OpenGL** libraries are correctly linked in the project settings.  

---

## **Steps to Change the Music Path**  

1. **Open** `main.cpp` in any text editor or IDE.  
2. **Locate** the line where the music file is loaded, e.g.:  
   ```cpp
   PlaySound("path/to/music.wav", NULL, SND_LOOP | SND_ASYNC);
   ```  
3. **Replace** `"path/to/music.wav"` with the correct file location:  

   **For Windows:** Use **double backslashes (`\\`)** or a **raw string**:  
     ```cpp
     PlaySound("C:\\Users\\YourName\\Music\\background.wav", NULL, SND_LOOP | SND_ASYNC);
     ```  
    **For Linux/macOS:** Use a **relative or absolute path**:  
     ```cpp
     PlaySound("/home/yourname/Music/background.wav", NULL, SND_LOOP | SND_ASYNC);
     ```  
4. **Save** the file and **recompile** the project.  

---

## **CONTROL INSTRUCTIONS**  

- **Keys:** `0`, `1`, `2`, `3`  
- **Function:** `handleInput`  
- **Purpose:** Switch between different scenes.  

| **Key** | **Action** |
|---------|-----------|
| **0**   | Switches to **Scene 0** |
| **1**   | Switches to **Scene 1** |
| **2**   | Switches to **Scene 2** |
| **3**   | Switches to **Scene 3** |

---

## **Scene 0 Controls**  

- **Function:** `keyboardScene0`  
- **Purpose:** Control ship movement.  

| **Key** | **Action** |
|---------|-----------|
| **A**   | Move the ship **left** |
| **G**   | Move the ship **right** |

---

## **Scene 1 Controls**  

- **Function:** `keyboardScene1`  
- **Purpose:** Control **day/night mode**, submarine movement, and exit the program.  

| **Key** | **Action** |
|---------|-----------|
| **D** / **d** | Toggle **day/night mode** |
| **G** / **g** | Start moving the **submarine to the right** |
| **Esc** | **Exit** the program |

---

## **Scene 2 Controls**  

- **Function:** `keyboardScene2`  
- **Purpose:** Control **submarine movement and speed**.  

| **Key** | **Action** |
|---------|-----------|
| **W**   | Move the submarine **up** |
| **S**   | Move the submarine **down** |
| **A**   | Move the submarine **left** |
| **G**   | Move the submarine **right** |
| **Spacebar** | **Stop** the submarine |
| **Enter** | **Start** the submarine movement |

---

## **Scene 3 Controls**  

- **Function:** `keyboardScene3`  
- **Purpose:** Control **submarine movement and speed**.  

| **Key** | **Action** |
|---------|-----------|
| **W**   | Move the submarine **up** |
| **S**   | Move the submarine **down** |
| **A**   | Move the submarine **left** |
| **G**   | Move the submarine **right** |
| **Spacebar** | **Stop** the submarine |
| **Enter** | **Start** the submarine movement |

---


![image](https://github.com/user-attachments/assets/0e751727-d5db-4379-ac82-210568e1df48)


