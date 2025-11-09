<h1>VTQ 2025 Hackathon Submission</h1>

<h3>Authors:</h3>
<p>Jeewant Choudhry (jeewant5@vt.edu), Lebone Boywer (lboyer05@vt.edu), Rhett Henderson (rhetthenderson@vt.edu)</p>

---

### 🧩 Overview
This repository contains our submission for the **Virginia Tech Quantum (VTQ) Hackathon 2025**, focused on building and optimizing quantum algorithms for efficient amplitude estimation and circuit depth reduction.

---

### ⚙️ Problem Statement
The goal was to improve the estimation of a probability parameter **p** by combining ideas from **Grover’s Algorithm** and **Quantum Amplitude Estimation (QAE)**.  
We aimed to reduce the number of **CNOT gates** (a major cost in real quantum hardware) while maintaining low **RMSE (Root Mean Square Error)** in the final probability estimates.

---

### 💡 Approach
1. Implemented a **parameterized quantum circuit (ansatz)** inspired by Grover’s operator.  
2. Used **Qiskit** to simulate and measure circuit performance under different CNOT budgets.  
3. Optimized rotation parameters using **classical optimizers (L-BFGS-B)** from SciPy.  
4. Generated **RMSE vs CNOT count** plots to visualize accuracy–efficiency tradeoffs.  
5. Compared full-depth circuits against **shallow ansatz** versions to achieve faster convergence with fewer operations.

---

### 🧠 Concepts Covered
- Grover’s Search Algorithm  
- Quantum Amplitude Estimation  
- Parameterized Quantum Circuits (Ansatz Design)  
- Quantum Statevector and Overlap Optimization  
- CNOT Gate Budget Analysis  
- Hybrid Classical–Quantum Optimization Techniques  

---

### 🧰 Tools and Libraries
- **Qiskit** – Circuit design, simulation, and measurement  
- **SciPy (optimize)** – Parameter tuning and minimization  
- **NumPy** – Numerical computations and vector manipulation  
- **Matplotlib** – RMSE visualization and performance plotting  

---

### 📊 Results
- Achieved faster RMSE convergence using shallow parameterized circuits.  
- Reduced total CNOT count by over 40% while maintaining similar accuracy.  
- Validated effectiveness of hybrid optimization for large qubit systems (6-qubit tests).

---

### 🔍 Future Scope
- Extend optimization to noisy simulators and real IBM Quantum devices.  
- Explore adaptive ansatz depth selection based on circuit fidelity thresholds.  
- Generalize approach for broader amplitude estimation problems in finance and physics.

---

### 📁 Repository Contents
- `1o_to_2o_code.ipynb` – Code for parameterized circuit and amplitude estimation tasks  
- `task3_shallow_rmse_plot.ipynb` – Final task integrating shallow circuits and plotting results  
- `report.pdf` – Detailed explanation of methods and results  

---

<p align="center"><i>Developed as part of the VTQ 2025 Hackathon at Virginia Tech</i></p>
