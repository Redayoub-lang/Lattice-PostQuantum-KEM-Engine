# Ring-LWE Post-Quantum Key Encapsulation Engine

![Python 3](https://img.shields.io/badge/Language-Python%203.10-blue)
![Mathematics](https://img.shields.io/badge/Domain-Applied%20Mathematics%20%26%20Cryptography-purple)
![Developer](https://img.shields.io/badge/Developer-Ayoub%20Lahmar-brightgreen)

A lattice-based cryptographic key encapsulation engine relying on the hardness of the **Ring Learning With Errors (Ring-LWE)** problem over quotient polynomial rings.

Implemented by **Ayoub Lahmar** ([@Redayoub-lang](https://github.com/Redayoub-lang)).

## 📐 Mathematical Formulation

Cryptographic operations are executed over the quotient polynomial ring \(R_q\):

$$
R_q = \mathbb{Z}_q[x] / (x^n + 1)
$$

Given public polynomial \(a \in R_q\), secret key \(s \in R_q\), and discrete Gaussian noise \(e \sim \chi(\sigma)\), the public key component \(b\) is generated via polynomial convolution:

$$
b = (a \cdot s + e) \pmod{q, x^n + 1}
$$

## 💻 Build & Run

```bash
python lattice_kem.py
