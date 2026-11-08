<div align="center">

# QuantumCryptography at Qiskit OSU

Qiskit Fall Fest 2026 at The Ohio State University

</div>

---

## Overview

Quantum computers change what it means for a message to be secure. Algorithms like Shor's threaten the public-key systems the internet runs on today, while quantum mechanics itself offers new ways to protect information. This organization explores both sides through a single Jupyter notebook built with [Qiskit](https://qiskit.org).

The notebook walks through the core ideas of quantum cryptography with runnable circuits and simulations, so each concept can be seen working rather than only described.

## Repositories

| Repository | Description |
|------------|-------------|
| [`.github`](https://github.com/QuantumCryptography-at-Qiskit-OSU/.github) | Organization profile |
| `Submission` | The Final submission repository |

## Setting Up a Python Environment

These steps create an isolated Python environment and connect it to Jupyter so the notebook runs with the right packages. Python 3.9 or newer is required.

**1. Clone the repository**

```bash
git clone https://github.com/QuantumCryptography-at-Qiskit-OSU/Submission.git
cd Submission
```

**2. Create a virtual environment**

```bash
python -m venv .venv
```

**3. Activate it**

```bash
# macOS / Linux
source .venv/bin/activate

# Windows (PowerShell)
.venv\Scripts\Activate.ps1
```

**4. Install the dependencies**

```bash
pip install --upgrade pip
pip install qiskit qiskit-aer matplotlib pylatexenc jupyter ipykernel
```

**5. Register the environment as a Jupyter kernel**

```bash
python -m ipykernel install --user --name qiskit-osu --display-name "Python (Qiskit OSU)"
```

**6. Launch Jupyter and open the notebook**

```bash
jupyter notebook
```

Open the notebook, then choose **Kernel > Change Kernel > Python (Qiskit OSU)**. In JupyterLab, use the kernel name in the top right corner instead. In VS Code, click **Select Kernel** and pick the `.venv` interpreter.

**7. Verify the setup**

Run this in the first cell of the notebook. It should print a version number without errors.

```python
import qiskit
print(qiskit.__version__)
```
