# Hybrid Quantum–Classical Machine Learning (QML)

This repository contains a learning-oriented implementation of a **hybrid quantum–classical machine learning model** using **Cirq** and **TensorFlow Quantum**. The project was developed to gain experience with fundamental concepts in **quantum information processing**, including quantum state preparation, parameterized quantum circuits, entanglement, and measurement.

The model is applied to a **binary image classification task** using a reduced version of the Fashion-MNIST dataset. The focus of this project is on understanding the workflow and limitations of near-term quantum machine learning rather than achieving superior performance over classical methods.

---

## Motivation

With the current limitations of near-term quantum hardware (NISQ era), hybrid quantum–classical approaches are widely used to explore how quantum circuits can be integrated into classical learning pipelines. This project was undertaken to:

- Learn how classical data can be encoded into quantum states  
- Understand how parameterized quantum circuits act as trainable models  
- Explore measurement-based readout and hybrid optimization  
- Gain practical familiarity with quantum machine learning frameworks  

---

## Project Overview

The workflow implemented in this project consists of:

1. **Data preprocessing**
   - Selection of a binary classification task from Fashion-MNIST  
   - Dimensionality reduction to fit limited qubit resources  
   - Binarization of input data  

2. **Quantum data encoding**
   - Encoding classical binary features into quantum states using Cirq  
   - Explicit construction of quantum circuits for state preparation  

3. **Parameterized quantum circuit (PQC)**
   - Construction of a small trainable quantum circuit with entangling gates  
   - Use of symbolic parameters for variational learning  

4. **Hybrid training loop**
   - Measurement of expectation values from the quantum circuit  
   - Classical loss computation and optimization using Adam  
   - End-to-end hybrid quantum–classical training  

5. **Evaluation**
   - Performance evaluation on a held-out test set  
   - Discussion of limitations and observed behavior  

---

## Technologies Used

- Python  
- Cirq  
- TensorFlow Quantum  
- TensorFlow / Keras  
- NumPy  
- Matplotlib  

---

## Results (Brief)

The hybrid model achieves stable convergence on the binary classification task, demonstrating that simple parameterized quantum circuits can be trained using classical optimization techniques. The results highlight both the potential and current limitations of quantum machine learning in the NISQ era.

---

## Limitations and Future Work

- The model operates on a very small number of qubits due to hardware and simulation constraints  
- No claim of quantum advantage is made  
- Future extensions could include:
  - Alternative encoding schemes  
  - Different circuit architectures  
  - Noise-aware simulations  
  - Experiments on real quantum hardware  

---

## Learning Outcome

This project served as a hands-on introduction to quantum machine learning and helped build intuition for quantum circuits, entanglement, measurement, and hybrid optimization workflows.

---

