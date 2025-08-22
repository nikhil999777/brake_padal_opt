# Brake Pedal Optimization using Topology Driven Latticing

## 📖 Overview

This project focuses on the structural optimization of a vehicle brake pedal using **nTopology** software. The primary goal was to reduce the component's weight and material usage while ensuring its structural integrity under standard operating loads. This was achieved by applying topology optimization followed by a topology-driven latticing technique, exploring three different lattice structures.


---

## 🎯 Objective

The core objectives of this project were:
* To optimize the material distribution of a standard brake pedal model.
* To utilize **nTopology's Topology Driven Latticing** tool to create lightweight yet strong designs.
* To perform a comparative analysis of the results based on **stress**, **displacement**, and **percentage of weight reduction** for each design variation.

---

## ⚙️ Simulation Setup

The analysis was conducted under the following conditions to simulate real-world usage:

* **Load**: A static force of **200 N** was applied to the foot paddle in the negative Z-direction.
  <img width="395" height="385" alt="image" src="https://github.com/user-attachments/assets/1ad84319-0143-483f-a74a-cc81f906ee6e" />

* **Boundary Condition**: The fixed end of the pedal, where it pivots, was **fully constrained**, preventing any movement or rotation.
  <img width="327" height="306" alt="image" src="https://github.com/user-attachments/assets/60adad95-3d69-4fba-a6cf-75c78cf38fb0" />


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
* **Simple Cubic Lattice**: Achieved the **highest weight reduction** (33.05%) but at the cost of the **highest displacement** (24.90 mm), indicating lower stiffness. 
* **BCC Lattice**: Experienced the **highest maximum stress** (97.95 MPa), which could be a concern for material failure or fatigue over time. 
* **FCC Lattice**: Provided the most **balanced performance**. [cite_start]It offered a significant weight reduction (22.48%) while maintaining the **lowest displacement** (14.83 mm) and a low maximum stress (64.41 MPa), making it the most robust and stiffest design of the three. 

---

## 🖼️ Visualizations

#### Optimized Simple Cubic
*Stress Distribution*
![Stress plot for Simple Cubic lattice](<img width="803" height="461" alt="image" src="https://github.com/user-attachments/assets/51fbb7d9-f26b-4933-a9c7-3f52687bc53f" />
)
*Displacement Plot*
![Displacement plot for Simple Cubic lattice](<img width="755" height="461" alt="image" src="https://github.com/user-attachments/assets/48a7fd79-dcab-4870-8836-3691afc9b77a" />
)

#### Optimized BCC
*Stress Distribution*
![Stress plot for BCC lattice](<img width="812" height="466" alt="image" src="https://github.com/user-attachments/assets/a383d795-cc57-46a8-ba3c-5a7db0dae437" />
)
*Displacement Plot*
![Displacement plot for BCC lattice](<img width="810" height="457" alt="image" src="https://github.com/user-attachments/assets/9570752d-6b86-4e73-9725-e09626c27f5f" />
)

#### Optimized FCC
*Stress Distribution*
![Stress plot for FCC lattice](<img width="811" height="477" alt="image" src="https://github.com/user-attachments/assets/20c05a10-5a35-4a87-9b03-4344b034ac7a" />
)
*Displacement Plot*
![Displacement plot for FCC lattice](<img width="807" height="480" alt="image" src="https://github.com/user-attachments/assets/a4b1d92e-fd34-43a1-b419-9b1e58351ce7" />
)

---

## ✅ Conclusion

This project successfully demonstrates the effectiveness of topology-driven latticing for lightweighting mechanical components. The **Face-Centered Cubic (FCC) lattice structure emerged as the superior choice** for this brake pedal application, providing the best combination of high stiffness (lowest displacement), manageable stress levels, and significant weight savings. Such optimized designs are ideal for **additive manufacturing (3D printing)**.
