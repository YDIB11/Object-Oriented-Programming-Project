# Object-Oriented Programming — Robot Cleaner Simulation

A C++ OOP project that simulates a robot clearing particles on a map, with a lightweight graphical layer to visualize state and interact with the run. The code showcases encapsulation, composition, and a clean split between simulation, graphics, and input.

> Build system: Makefile · Language: C++

---

## ✨ Features
- Domain objects: Robot, Particule, Shape, Simulation, Message
- Simple graphics + input (graphic.*, gui.*)
- Deterministic step loop (run or step-by-step)
- Headers (.h) for APIs, implementations (.cc) for logic

---

## 🗂️ Project Layout (overview)

.  
├─ Makefile  
├─ constantes.h  
├─ projet.cc             (entry point)  
├─ simulation.{h,cc}     (world state & update loop)  
├─ robot.{h,cc}          (robot behavior)  
├─ particule.{h,cc}      (map particles)  
├─ shape.{h,cc}          (geometric primitives)  
├─ gui.{h,cc}            (input / small UI)  
├─ graphic.{h,cc}        (drawing primitives)  
└─ message.{h,cc}        (UI/system messaging)


---

## ⚙️ Build & Run

Linux / macOS
    make
    ./projet

If you want stricter warnings (if your Makefile allows overrides):
    make clean
    make CXXFLAGS='-O2 -Wall -Wextra -pedantic'

---

