# MSc Dissertation Project Code

Code to test and benchmark the performance of cryptographic libraries providing MLS protocol and threshold signatures.  

**General Code Development Process**

1. Download libary from specified Git repository.
2. Run benchmark/test code supplied with library to confirm functionality.
3. Use AI (Google Gemini / Microsoft Copilot) to modify code to required functionality and to apply perfomrnace measurement/benchmarking code.

**Implementations**

OpenMLS - Rust implementation of the MLS protocol. 
  - My repo: https://github.com/RochP-Lab/MLS-OpenMLS
  - messagingbatch.rs allows testing of multiple ciphersuites and message sizes, with various performance metrics recorded.

mlspp - C++ implementation of the MLS protocol. 
  - My repo: https://github.com/RochP-Lab/MLS-mlspp
  - main.cpp and CMakeLists.txt compile to produce benchmark_runner, this tests multiple ciphersuites and messages sizes, with various performance metrics recorded.

Kryptology - Golang implementation of FROST signatures using Ed25519 curve. 
  - My repo: -  https://github.com/RochP-Lab/DKG-Kryptology
  - main.go - Code to benchmark preformance of library
  - ???. Code to prove test libraries BFT

Bank Italia - C implementation of FROST signatures using secp256k1 curve.
  - My repo: https://github.com/RochP-Lab/DKG-BankItalia

