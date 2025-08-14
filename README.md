# MSc Dissertation Project Code

Code to test and benchmark the performance of cryptographic libraries providing MLS protocol and threshold signatures.  

**General Code Development Process**

1. Download libary from specified Git repository.
2. Run benchmark/test code supplied with library to confirm functionality.
3. Use AI (Google Gemini / Microsoft Copilot) to modify code to required functionality and to apply perfomrnace measurement/benchmarking code.

**Implementations**

MLS - OpenMLS - Rust implementation of the MLS protocol. 
  - 

MLS - MLSpp - C++ implementation of the MLS protocol. 
  - 
  - main.cpp and CMakeLists.txt compile to produce benchmark_runner, this tests multiple ciphersuites and messages sizes, with various performance metrics recorded.

FROST - Kryptology - Golang implementation of FROST signatures using Ed25519 and secp256k1 curves. 
-  
  - main.go - Code to benchmark preformance of library
  - ???. Code to prove test libraries BFT

FROST - Bank Italia - C implementation of FROST signatures using secp256k1 curve.
- 
  - DKG and trusted dealer benchmarks.
 

FROST - Zcash Foundation - Rust implementation of FROST signatures using Ed25519 curve.
- 

BLS - BLSTRS - Rust implementation of BLS signatures using BLS... curv
- DKG implementation

Herumi - BLS - C++ implementation of BLS signatures
- Trusted dealer implementation






