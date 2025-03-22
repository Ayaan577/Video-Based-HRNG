# Video-Based Hardware Random Number Generator (HRNG)

## Overview
This project implements a Video-Based Hardware Random Number Generator (HRNG) leveraging video frames as a source of entropy. The randomness is extracted through a series of processing steps, validated using statistical methods, and utilized for cryptographic key generation. The project demonstrates how natural entropy sources can be integrated into cryptographic systems for enhanced security.

---

## Features
- **Randomness Extraction**:
  - Processes video frames to extract raw bitstreams.
  - Applies debiasing techniques like Von Neumann correction, XOR folding, and SHA-256 hashing.
- **Randomness Validation**:
  - Conducts statistical randomness tests (Frequency Test, Runs Test, Shannon Entropy).
- **Cryptographic Key Generation**:
  - Generates 256-bit cryptographic keys.
  - Demonstrates encryption and decryption using AES-256 in CBC mode.

---

## Requirements
- Python 3.7+
- Dependencies:
  - `opencv-python`
  - `numpy`
  - `matplotlib`
  - `scipy`
  - `pycryptodome`

Install dependencies using:
```bash
pip install opencv-python numpy matplotlib scipy pycryptodome
