# MSc Dissertation Project Code

Code to test and benchmark the performance of various cryptographic libraries, currently: 

OpenMLS - Rust imnplementation of the MLS protocol. 
  - messagingbatch.rs allows testing of multiple ciphersuites and message sizes, with various performance metrics recorded.

mlspp - C++ implementation of the MLS protocol. 
  - main.cpp and CMakeLists.txt compile to produce benchmark_runner, this tests multiple ciphersuites and messages sizes, with various performance metrics recorded.

Kryptology - Golang implementation of FROST signatures using Ed25519 curve. 
  -  main.go - Code to benchmark preformance of library
  -   - Code to prove test libraries BFT

**Bank Italia** **- **C implementation of FROST signatures using secp256k1 curve.
  -     

**Code Development Process**

1. Stared with large_groups.rs supplied with OpenMLS as example code to demo the performance of handshake operations. 
2. Critical performance measurement is time to encrypt/decrypt application messages, this is lacking from large_groups.rs. Used Google Gemini to iteratively develop code that tested .create_message and .decrypt_message to encrypt and then decrypt messages.
3. Expanded code to cycle through different messages and more reliably measure performance (1000 iterations, warmup iterations).
4. mlspp library isn't supplied with benchmarking/example code. Used Gemini to develop an equivalent test harness that ran the equivalent tests in C++ for this library.

