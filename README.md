Flexible Representation of Quantum Images (FRQI) with Quantum Watermarking on IBM Brisbane 127-Qubit Processor
Overview
This project demonstrates the experimental realization of Flexible Representation of Quantum Images (FRQI) with simultaneous quantum watermarking on IBM Quantum's 127-qubit Brisbane processor.

We optimize quantum angle perturbations and introduce hardware-aware error mitigation strategies, achieving dual image representation and watermark encoding under Noisy Intermediate-Scale Quantum (NISQ) hardware constraints.

Key Features
FRQI-based Image Encoding:
Efficient representation of 
2
×
2
2×2 grayscale images using quantum states.

Transparent Quantum Watermarking:
Watermarked regions showed angular perturbations 
Δ
=
0.203
 
rad
Δ=0.203rad, while non-watermarked regions showed 
Δ
=
−
0.216
 
rad
Δ=−0.216rad (Welch's t-test: 
𝑡
=
7.58
t=7.58, 
𝑝
=
0.0564
p=0.0564).

Advanced Error Mitigation:

Mthree (M3) Readout Correction with synthetic calibration fallback.

Dynamical Decoupling Sequences for 
𝑇
1
T 
1
​
  preservation.

Sabre-Optimized Circuit Routing to minimize hardware noise.

Quantum Noise Characterization:

Measurement infidelity reduced from 38% to 2.8%.

ECR gate error rates at 
8.093
×
10
−
3
8.093×10 
−3
  per gate.

𝑇
1
T 
1
​
  decoherence times of approximately 
230.85
 
𝜇
𝑠
230.85μs.

Performance Metrics:

Peak Signal-to-Noise Ratio (PSNR): 17.83 dB

Mean Squared Error (MSE): 1070.54

Quantum State Fidelity (QSF): Improved by 38% after mitigation.

Quantum Distortion Index (QDI): 0.42 indicating moderate coherent distortion.

Motivation
Current NISQ devices introduce significant noise that affects angular precision critical for quantum imaging and watermarking tasks. This project addresses:

The gap between theoretical models and hardware realities.

Development of noise-adaptive quantum imaging protocols.

Foundations for secure medical and defense imaging applications using quantum hardware.

Technologies Used
Qiskit (IBM Quantum SDK)

Python 3.11+

IBM Quantum Platform (Brisbane 127-qubit device)

Matplotlib, NumPy for data visualization and analysis
