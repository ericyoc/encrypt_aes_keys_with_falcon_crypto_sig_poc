# Post-Quantum Image Encryption and Signature Using FALCON

This project implements a multi-level approach to image encryption and signing using post-quantum cryptographic techniques, with a focus on the FALCON (Fast-Fourier Lattice-based Compact Signatures over NTRU) algorithm for digital signatures.

## Motivating Articles and Related Work
Rawal, B. S., & Biswas, A. (2024). A comprehensive survey of post-quantum cryptography and its implications. Engineering Science & Technology, 256-269.
https://ojs.wiserpub.com/index.php/EST/article/view/4169

Luc, N. Q., Nguyen, T. T., Quach, D. H., Dao, T. T., & Pham, N. T. (2023). Building Applications and Developing Digital Signature Devices based on the Falcon Post-Quantum Digital Signature Scheme. Engineering, Technology & Applied Science Research, 13(2), 10401-10406.
https://ojs.wiserpub.com/index.php/EST/article/view/4169

FALCON
https://falcon-sign.info/

## Overview

This system combines various cryptographic techniques to provide a robust, post-quantum secure method for image encryption and authentication. It utilizes 2D Discrete Wavelet Transform (DWT), Advanced Encryption Standard (AES), Learning With Errors (LWE), and the FALCON signature algorithm.

## Features

- Standard and Enhanced 2D-DWT for image transformation
- AES encryption for initial data security
- LWE encryption for post-quantum security
- FALCON digital signatures for post-quantum authentication
- Multi-level approach combining various cryptographic techniques
- Performance analysis using Mean Squared Error (MSE)

## Major Concepts

1. **2D Discrete Wavelet Transform (DWT)**: Used for image transformation, providing both standard and enhanced versions.
2. **AES Encryption**: Provides initial encryption of the transformed image data.
3. **Learning With Errors (LWE)**: A post-quantum lattice-based encryption scheme used to encrypt the AES ciphertext.
4. **FALCON Signatures**: A post-quantum digital signature algorithm used for image authentication.
5. **Multi-level Security**: Combines different techniques to enhance overall security.

## FALCON Algorithm

The FALCON (Fast-Fourier Lattice-based Compact Signatures over NTRU) algorithm is a key component of this system, providing post-quantum secure digital signatures. FALCON is:

- Based on the hardness of the NTRU lattice problem
- Designed to be fast and have compact signatures
- Part of the NIST Post-Quantum Cryptography standardization process

In this project, FALCON is used to:
1. Generate key pairs (secret and public keys)
2. Sign the processed image data
3. Verify the signature to ensure image authenticity

The implementation includes features such as:
- Automatic retrying of signature generation if the signature norm is too large
- Conversion between image formats and byte strings for signing
- Integration with the overall multi-level encryption process
- 
## Disclaimer
The Python code is for academic and research purposes only.
