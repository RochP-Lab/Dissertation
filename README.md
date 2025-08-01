# MSc Dissertation Project Code

Code to test and benchmark the performance of various cryptographic libraries, currently: 

OpenMLS - Rust imnplementation of the MLS protocol. messagingbatch.rs allows testing of multiple ciphersuites and message sizes, with various performance metrics recorded.

mlspp - C++ implementation of the MLS protocol. main.cpp and CMakeLists.txt compile to produce benchmark_runner, this tests multiple ciphersuites and messages sizes, with various performance metrics recorded. 

