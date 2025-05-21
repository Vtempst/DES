# DES in Verilog on Digilent Nexys A7

A from-scratch Verilog implementation of the Data Encryption Standard (DES), synthesized and deployed on a Digilent Nexys A7 FPGA. Includes a UART interface that streams 64-bit plaintext and ciphertext to Tera Term for live verification.

## 🚀 Features
- **Complete DES core**: Initial Permutation, 16 Feistel rounds (including S-boxes, expansion, P-permutation), key schedule, and final permutation.
- **On-the-fly key scheduling**: Generates all 16 subkeys from a 64-bit user key (56 bits + parity).
- **UART validation**: Sends/receives 64-bit words over UART via Tera Term for immediate plaintext/ciphertext checks.
- **FPGA-ready**: Constraints and Vivado project files included for the Nexys A7 (Artix-7).
