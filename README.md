# 🚀 Quantum Computing & Qiskit Introduction

Welcome to the **Quantum Computing Introduction** repository! This repository contains practical introductory examples of [Qiskit](https://qiskit.org/) and a guide to setting up your environment using **Miniconda**. 

Here, you will step into the fascinating world of quantum mechanics, qubits, superposition, entanglement, and quantum gates!

---

## 🎯 What's in this Repository?

1. **`00_Miniconda_Setup_Presentation.md`**
   - A step-by-step presentation on how to install Miniconda.
   - Basics of creating and managing virtual environments.
   - Setting up a specialized environment for Jupyter Notebooks and Qiskit.
   
2. **`01_Qiskit_Introduction.ipynb`**
   - An interactive, visually rich Jupyter Notebook.
   - Explanations of basic quantum gates (Pauli X, Y, Z, Hadamard, CNOT).
   - Practical, runnable examples of creating and simulating quantum circuits with Qiskit.

---

## 🛠️ Getting Started

Follow these steps to get your environment ready for Quantum Computing!

### Step 1: Clone the Repository
Open your terminal or command prompt and clone this repository to your local machine:
```bash
git clone <repository_url>
cd <repository_folder_name>
```

### Step 2: Read the Setup Presentation
Review the **`00_Miniconda_Setup_Presentation.md`** file. It covers how to download Miniconda and why we use it for Python development.

### Step 3: Create the Quantum Environment
If you have Miniconda installed, simply open your **Anaconda Prompt** (Windows) or Terminal (Mac/Linux) and run:
```bash
# Create a new environment named 'qiskit-env' with Python 3.10
conda create -n qiskit-env python=3.10 -y

# Activate the environment
conda activate qiskit-env

# Install Jupyter and Qiskit
pip install jupyter qiskit qiskit-aer matplotlib pylatexenc
```

### Step 4: Launch Jupyter Notebook
Inside the activated environment and the repository folder, run:
```bash
jupyter notebook
```
This will open Jupyter in your browser. Click on **`01_Qiskit_Introduction.ipynb`** and start your quantum journey!

---

## 💡 About Qiskit
[Qiskit](https://qiskit.org/) is an open-source SDK for working with quantum computers at the level of pulses, circuits, and application modules. It accelerates the development of quantum applications by providing the complete set of tools needed for quantum computing research and education.

Happy coding, and welcome to the quantum era! 🌌
