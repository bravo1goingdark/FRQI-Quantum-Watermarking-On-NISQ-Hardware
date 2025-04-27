# Flexible Representation of Quantum Images (FRQI) with Quantum Watermarking on IBM Brisbane 127-Qubit Processor

## Overview

This project demonstrates the **experimental realization** of **Flexible Representation of Quantum Images (FRQI)** with **simultaneous quantum watermarking** on IBM Quantum's 127-qubit Brisbane processor.

We optimize quantum angle perturbations and introduce hardware-aware error mitigation strategies, achieving dual image representation and watermark encoding under Noisy Intermediate-Scale Quantum (NISQ) hardware constraints.

## Key Features

- **FRQI-based Image Encoding:**  
  Efficient representation of \(2 \times 2\) grayscale images using quantum states.

- **Transparent Quantum Watermarking:**  
  Watermarked regions showed angular perturbations \(\Delta = 0.203\,\text{rad}\), while non-watermarked regions showed \(\Delta = -0.216\,\text{rad}\) (Welch's t-test: \(t = 7.58\), \(p = 0.0564\)).

- **Advanced Error Mitigation:**  
  - **Mthree (M3) Readout Correction** with synthetic calibration fallback.
  - **Dynamical Decoupling Sequences** for \(T_1\) preservation.
  - **Sabre-Optimized Circuit Routing** to minimize hardware noise.

- **Quantum Noise Characterization:**  
  - Measurement infidelity reduced from 38% to 2.8%.
  - ECR gate error rates at \(8.093 \times 10^{-3}\) per gate.
  - \(T_1\) decoherence times of approximately \(230.85\,\mu s\).

- **Performance Metrics:**  
  - Peak Signal-to-Noise Ratio (PSNR): **17.83 dB**  
  - Mean Squared Error (MSE): **1070.54**  
  - Quantum State Fidelity (QSF): **Improved by 38%** after mitigation.
  - Quantum Distortion Index (QDI): **0.42** indicating moderate coherent distortion.

## Motivation

Current NISQ devices introduce significant noise that affects angular precision critical for quantum imaging and watermarking tasks. This project addresses:

- The **gap between theoretical models** and **hardware realities**.
- Development of **noise-adaptive quantum imaging protocols**.
- Foundations for **secure medical and defense imaging applications** using quantum hardware.

## Technologies Used

- **Qiskit** (IBM Quantum SDK)
- **Python 3.11+**
- **IBM Quantum Platform** (Brisbane 127-qubit device)
- **Matplotlib**, **NumPy** for data visualization and analysis

## How to Run

> **Note:** This project was run on IBM Quantum hardware. To reproduce, you must have access to IBMQ resources.

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/quantum-frqi-watermarking.git
    cd quantum-frqi-watermarking
    ```

2. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Set up your IBM Quantum credentials:
    ```python
    from qiskit import IBMQ
    IBMQ.save_account('YOUR_IBM_QUANTUM_API_TOKEN')
    ```

4. Run the FRQI encoding and watermarking script:
    ```bash
    python frqi_watermarking.py
    ```

## Results

| Metric | Value |
|:-------|:------|
| PSNR | 17.83 dB |
| MSE | 1070.54 |
| Quantum State Fidelity (post-mitigation) | 0.61 |
| Quantum Distortion Index (QDI) | 0.42 |
| Measurement Infidelity (post-correction) | 2.8% |

## Citation

If you use or reference this work, please cite:

> Flexible Representation of Quantum Images and Quantum Watermarking: Angle Perturbations on Noisy Intermediate-Scale Quantum Hardware (2025)

## License

This project is licensed under the [MIT License](LICENSE).
