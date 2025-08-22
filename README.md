# Brake Pedal Optimization using Topology Driven Latticing

## 📖 Overview

This project focuses on the structural optimization of a vehicle brake pedal using **nTopology** software. The primary goal was to reduce the component's weight and material usage while ensuring its structural integrity under standard operating loads. This was achieved by applying topology optimization followed by a topology-driven latticing technique, exploring three different lattice structures.


---

## 🎯 Objective

The core objectives of this project were:
* [cite_start]To optimize the material distribution of a standard brake pedal model. [cite: 3]
* [cite_start]To utilize **nTopology's Topology Driven Latticing** tool to create lightweight yet strong designs. [cite: 4]
* [cite_start]To perform a comparative analysis of the results based on **stress**, **displacement**, and **percentage of weight reduction** for each design variation. [cite: 7]

---

## ⚙️ Simulation Setup

The analysis was conducted under the following conditions to simulate real-world usage:

* [cite_start]**Load**: A static force of **200 N** was applied to the foot paddle in the negative Z-direction. [cite: 5]
* [cite_start]**Boundary Condition**: The fixed end of the pedal, where it pivots, was **fully constrained**, preventing any movement or rotation. [cite: 6]

---

## 🔬 Methodology

The optimization process involved infilling the brake pedal's solid body with three distinct types of lattice structures. A static structural analysis was then performed on each of the three resulting models:

1.  **Optimized with Simple Cubic Lattice**
2.  **Optimized with Body-Centered Cubic (BCC) Lattice**
3.  **Optimized with Face-Centered Cubic (FCC) Lattice**

The performance of each design was evaluated to find the optimal balance between weight and structural performance.

---

## 📊 Results and Analysis

The final results from the static structural analysis for each lattice type are summarized below.

| Ribbing Type | Max Stress (MPa) | Max Displacement (mm) | % Weight Reduction |
| :--- | :---: | :---: | :---: |
| Optimized Simple Cubic | 64.30 | 24.90 | **33.05%** |
| Optimized BCC | **97.95** | 18.32 | 29.20% |
| Optimized FCC | 64.41 | **14.83** | 22.48% |

### Key Observations:
* [cite_start]**Simple Cubic Lattice**: Achieved the **highest weight reduction** (33.05%) but at the cost of the **highest displacement** (24.90 mm), indicating lower stiffness. 
* [cite_start]**BCC Lattice**: Experienced the **highest maximum stress** (97.95 MPa), which could be a concern for material failure or fatigue over time. 
* **FCC Lattice**: Provided the most **balanced performance**. [cite_start]It offered a significant weight reduction (22.48%) while maintaining the **lowest displacement** (14.83 mm) and a low maximum stress (64.41 MPa), making it the most robust and stiffest design of the three. 

---

## 🖼️ Visualizations

#### Optimized Simple Cubic
*Stress Distribution*
![Stress plot for Simple Cubic lattice](<URL_to_Simple_Cubic_Stress_Image.png>)
*Displacement Plot*
![Displacement plot for Simple Cubic lattice](<URL_to_Simple_Cubic_Displacement_Image.png>)

#### Optimized BCC
*Stress Distribution*
![Stress plot for BCC lattice](<URL_to_BCC_Stress_Image.png>)
*Displacement Plot*
![Displacement plot for BCC lattice](<URL_to_BCC_Displacement_Image.png>)

#### Optimized FCC
*Stress Distribution*
![Stress plot for FCC lattice](<URL_to_FCC_Stress_Image.png>)
*Displacement Plot*
![Displacement plot for FCC lattice](<URL_to_FCC_Displacement_Image.png>)

---

## ✅ Conclusion

This project successfully demonstrates the effectiveness of topology-driven latticing for lightweighting mechanical components. The **Face-Centered Cubic (FCC) lattice structure emerged as the superior choice** for this brake pedal application, providing the best combination of high stiffness (lowest displacement), manageable stress levels, and significant weight savings. Such optimized designs are ideal for **additive manufacturing (3D printing)**.
