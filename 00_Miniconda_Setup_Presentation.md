---
marp: true
theme: default
class: lead
paginate: true
backgroundColor: #1E1E1E
color: #FFFFFF
header: "**Quantum Environment Setup Guide**"
footer: "Quantum Computing Introduction | Setting up Miniconda & Qiskit"
---

# 🚀 Setting Up Your Quantum Environment
## A Guide to Miniconda, Virtual Environments, and Jupyter
---

## 🎯 Why Do We Need This?

When working with Python, particularly in data science and quantum computing:
- We use **many libraries** (like Qiskit, Numpy, Matplotlib).
- Different projects require **different versions** of these libraries.
- Installing everything globally can cause **version conflicts** and break your system.

**The Solution:** 📦 **Virtual Environments**
A virtual environment is an isolated workspace for a specific project. 

---

## 🐍 What is Miniconda?

**Miniconda** is a free minimal installer for conda. It is a small, bootstrap version of Anaconda that includes only conda, Python, the packages they depend on, and a small number of other useful packages.

**Why Miniconda instead of full Anaconda?**
- 🍃 **Lightweight:** Takes up very little disk space.
- ⚡ **Fast:** Installs quickly.
- 🛠️ **Customizable:** You only install the packages you actually need.

---

## 📥 Step 1: Downloading Miniconda

1. Go to the official Miniconda Download Page:
   👉 **[https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)**
2. Choose the correct installer for your Operating System:
   - **Windows:** Download the `.exe` installer (64-bit).
   - **macOS:** Download the `.pkg` or `.sh` installer (check if you have Intel or Apple Silicon/M1/M2).
   - **Linux:** Download the `.sh` installer.

---

## 🛠️ Step 2: Installation

### 🪟 Windows Setup
1. Double click the `.exe` file.
2. Follow the prompt (Next > I Agree > Just Me).
3. Choose the destination folder.
4. **Important:** Leave "Add Miniconda3 to my PATH environment variable" **unchecked** (Recommended).
5. Click **Install**.
6. Once finished, open the start menu and search for **Anaconda Prompt (Miniconda3)**. This is your new command line for Python!

*(macOS/Linux users can typically run the `.sh` script from their terminal and follow the prompts).*

---

## 🧪 Step 3: Basics of Virtual Environments

Now that you have Miniconda, let's learn the basic commands. Open your **Anaconda Prompt** (or Terminal).

**Check conda is working:**
```bash
conda --version
```

**See a list of your environments:**
```bash
conda env list
```
*(You will only see `base` right now)*

---

## 🏗️ Step 4: Creating Our Qiskit Environment

Let's create a dedicated environment for our Quantum Computing work. We will name it **`qiskit-env`** and use Python 3.10.

Run this command:
```bash
conda create --name qiskit-env python=3.10 -y
```

Congratulations! You have just created an isolated workspace.

---

## 🔌 Step 5: Activating the Environment

To start using this environment, you must **activate** it. 

Run:
```bash
conda activate qiskit-env
```

Notice how your prompt changes from `(base)` to `(qiskit-env)`. Everything we install now will only affect this environment!

*(To leave an environment later, you can use `conda deactivate`)*

---

## 💻 Step 6: Installing Jupyter and Qiskit

Now that we are *inside* `qiskit-env`, let's install the tools we need for the notebook.

We will use `pip` (the Python package installer) which is included in our environment.

Run this command to install Jupyter, Qiskit, and visualization tools:
```bash
pip install jupyter qiskit qiskit-aer matplotlib pylatexenc
```
*Wait a few moments for the download and installation to complete.*

---

## 🚀 Step 7: Launching Jupyter Notebook

You are all set! Let's start coding.

1. In your Anaconda Prompt, navigate to the folder where you cloned the repository.
   *(E.g., `cd path/to/repo`)*
2. Run the Jupyter Notebook server:
```bash
jupyter notebook
```
3. Your web browser will open automatically.
4. Click on **`01_Qiskit_Introduction.ipynb`** and let's explore Quantum mechanics! 🎉
