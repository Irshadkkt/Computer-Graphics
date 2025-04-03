# Computer-Graphics
Contains various computer graphics projects, including implementations of transformations, rendering algorithms, and visualization techniques.

Here's a complete **README** file covering all the codes you provided, including **Hermite Curve, DDA Line Drawing, and Midpoint Circle Algorithm**.  

---

# **Computer Graphics Algorithms in C++ (Turbo C++ BGI)**
This repository contains implementations of essential **computer graphics algorithms** using **Turbo C++ BGI Graphics Library**. The following algorithms are implemented:

✅ **Hermite Curve Generation**  
✅ **DDA Line Drawing Algorithm**  
✅ **Midpoint Circle Drawing Algorithm**  

Each algorithm is visualized using the **BGI graphics library**, making it suitable for **educational purposes and learning computer graphics fundamentals**.  

---

## **Table of Contents**
- [Prerequisites](#prerequisites)  
- [Setup & Installation](#setup--installation)  
- [Implemented Algorithms](#implemented-algorithms)  
  - [1. Hermite Curve](#1-hermite-curve)  
  - [2. DDA Line Drawing Algorithm](#2-dda-line-drawing-algorithm)  
  - [3. Midpoint Circle Algorithm](#3-midpoint-circle-algorithm)  
- [How to Run](#how-to-run)  
- [Future Enhancements](#future-enhancements)  

---

## **Prerequisites**
To run these programs, you need:  
✅ **Turbo C++ Compiler**  
✅ **BGI Graphics Library** (Path: `C:\\Turboc3\\BGI`)  

---

## **Setup & Installation**
1. Install **Turbo C++**.
2. Open Turbo C++ and set up **BGI graphics path**.
3. Copy and paste the required **C++ code** into Turbo C++.
4. Compile and execute the program.

---

## **Implemented Algorithms**

### **1. Hermite Curve**
📌 **Description**  
Hermite curves are cubic curves defined using **two endpoints** and **two tangent vectors**. This program:  
- Takes **four control points** (P1, P4) and two tangents (R1, R4).
- Uses **Hermite interpolation** to generate the curve.
- Renders the **curve on a Cartesian plane**.

📌 **Mathematical Formulation**  
\[
x(t) = (2t^3 - 3t^2 + 1) P1.x + (-2t^3 + 3t^2) P4.x + (t^3 - 2t^2 + t) R1.x + (t^3 - t^2) R4.x
\]
\[
y(t) = (2t^3 - 3t^2 + 1) P1.y + (-2t^3 + 3t^2) P4.y + (t^3 - 2t^2 + t) R1.y + (t^3 - t^2) R4.y
\]

📌 **How to Use**
- Enter the **four control points (x, y coordinates)**.
- The program **plots the Hermite curve** based on the given points.

---

### **2. DDA Line Drawing Algorithm**
📌 **Description**  
The **DDA (Digital Differential Analyzer) Algorithm** is an efficient method to draw a line between two points. It:
- Calculates the **smallest step increment** to **smoothly transition** between two points.
- Uses **floating-point arithmetic** for accuracy.
- Draws **Cartesian axes** as reference.

📌 **Algorithm Steps**
1. Calculate **dx = Xb - Xa** and **dy = Yb - Ya**.
2. Determine **steps** = max(|dx|, |dy|).
3. Compute **x-increment** and **y-increment**.
4. Plot **pixels iteratively** from `(Xa, Ya)` to `(Xb, Yb)`.

📌 **How to Use**
- Enter the **starting (Xa, Ya) and ending (Xb, Yb) points**.
- The program **draws a line** between these points using **DDA Algorithm**.

---

### **3. Midpoint Circle Algorithm**
📌 **Description**  
The **Midpoint Circle Algorithm** is used to draw circles efficiently using integer calculations. It:
- Uses **decision parameters** to determine the next pixel.
- Exploits **8-way symmetry** to plot a full circle.
- Draws **Cartesian coordinate axes**.

📌 **Algorithm Steps**
1. Initialize \( x = 0 \), \( y = R \), and **decision parameter** \( p = 1 - R \).
2. Check if the next pixel is **inside or outside** the circle.
3. Adjust \( p \) accordingly:
   - If \( p < 0 \), choose **right pixel**.
   - Else, choose **diagonal pixel**.
4. Repeat for **one octant** and reflect for **all 8 octants**.

📌 **How to Use**
- Enter **center coordinates (x, y)** and **radius**.
- The program **draws the circle** using **Midpoint Algorithm**.

---

## **How to Run**
1. Compile and run any of the above programs.
2. Enter the required **user inputs**.
3. Observe the **plotted graphics**.
4. Press any key to exit the graphics window.

---

## **Future Enhancements**
🚀 Implement **Bresenham’s Circle Algorithm** for better accuracy.  
🚀 Add **Bezier Curves** for more complex graphics rendering.  
🚀 Implement **interactive UI** for selecting shapes dynamically.  

---
