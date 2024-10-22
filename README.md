<div style="display: flex; justify-content: center; margin: 0 auto; width: 100%;">
  <img src="docs/media/Long Logo Banner - Readme.png" alt="Modubot: A Modular Robotics Project" style="width: 100%;"/>
</div>

---

**Modubot** is a modular robotics platform built around **cube-shaped modules**, each with a **dedicated PCB** designed for specific functions. These modules can serve as **regional controllers**, **motor controllers**, **sensor modules**, or other customizable components, allowing for a **flexible and adaptable robotic system**. The entire project is based on **STM32 microcontrollers**.

<div style="display: flex; justify-content: center; margin: 0 auto; width: 100%;">
  <img src="docs/media/BasicRobot_photo.jpg" alt="Image 1" style="width: 49%;"/>
  <img src="docs/media/GPM PCB.jpg" alt="Image 2" style="width: 49%;"/>
</div>

---

## **Goal:**

The vision for Modubot is to create a **flexible, modular platform** that promotes **hands-on learning** and **skill development**. By using **cube-based modules**, each with a unique **electronic function**, Modubot acts as a **test platform** for experimenting with:

- **Protocols**
- **Circuits**
- **PCB architecture**
- **Firmware**

This project is a chance to **apply and refine engineering knowledge** while exploring **creative possibilities in robotics**.

---

## **Roadmap:**
1. **✅ Design First Ever Module (General Purpose) - Accomplished**
2. **✅ Create a Simple 2-Wheel Robot with Remote Operation - Accomplished**
3. **🔲 Write Firmware for CAN-FD, IMU, UART GPS**
4. **🔲 Create a 2 Degrees of Freedom Arm**
5. **🔲 Design a Brushed/Stepper/BLDC Motor Controller Module (MCM)**
6. **🔲 Create a Miniature Buggy Rover**
7. **🔲 Design 2nd Version of the General Purpose Module (GPM)**
8. **🔲 Design Modular Drone (1x GPM + 4x MCM)**

---

## **Current Status:**

### **STAGE 2:**
The current phase features a **2-wheeled robot** designed as a **proof of concept**. It tests the **General Purpose Module (GPM v1)** along with:

- **SPI to NRF24L01** (used for remote control)
- **Servo control**

However, the **continuous servos** faced **tuning issues**, preventing the robot from driving straight, highlighting the need to shift towards **PID-controlled DC motors with encoders** for precise control.

<div style="display: flex; justify-content: center; margin: 0 auto; width: 100%;">
  <img src="docs/media/BasicRobot_photo.jpg" alt="Image 1" style="width: 28%;"/>
  <img src="docs/media/RemoteController.png" alt="Image 2" style="width: 49%;"/>
</div>


---

### **STAGE 1:**
The **first wave of designs** has been completed. The initial **PCB design** was kept **simple** to avoid unnecessary points of failure. It functions as intended, though there are some **design oversights**:

- It cannot handle **high current** (only 1-2 amps at 12V)
- Limited **resistance to back EMF**

These issues will be addressed in **version 2**, after learning more about system requirements.

<img src="docs/media/GPMv1_pcb_render.png" width="425"/> <img src="docs/media/GPMv1_schematic.png" width="425"/> <img src="docs/media/GPMv1_routing.png" width="425"/> 


The **3D-printed structure** has also been refined and is expected to remain unchanged unless major issues arise. For **quick connections** between modules and subcomponents (e.g., PCB bracket), **3D-printed Lego pins (scaled 1.25x)** are being used, and for more **permanent fixtures**, **M6 bolts** can be inserted in the same holes. Initially, **PETG** was used for printing, but due to **brittleness**, the material has been changed to **ABS**, which is more **ductile**.

![CAD of the board](docs/media/CubeFrameRender.png)
