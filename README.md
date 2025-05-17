# SYBAU — Smart Yogurt But Also DangeroUs

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

## Overview

SYBAU is a functional domain-specific language (DSL) that allows you to write expressive, easy-to-read code and automatically transforms it into highly optimized, high-performance C++.

The main goal is to simplify writing efficient code without requiring developers to master complex algorithmic or low-level optimization details. SYBAU applies static analysis, heuristics, and advanced optimizations to generate code that leverages:

- Optimal data structures based on detected access patterns (e.g., segment trees, sparse tables).  
- Memory alignment and automatic vectorization (SIMD).  
- Automatic parallelization with support for `std::execution` and OpenMP.  
- Machine learning for pattern detection and optimization suggestions (experimental).

---

## Features

- **Functional language:** clean and expressive syntax.  
- **Automatic optimization:** algorithm and data structure selection based on detected usage patterns.  
- **Low-level optimizations:** memory alignment, vectorization, cache-friendly transformations.  
- **Parallelization:** generates concurrent code with minimal developer effort.  
- **Extensible:** easy to add new analyses and optimizations.

---

## Getting Started

### Requirements

- Modern C++ compiler with C++17 or higher support (GCC, Clang, MSVC).  
- CMake 3.15+ for building.  
- [Optional] Python 3 for benchmarking scripts and ML components.

### Build

```bash
git clone https://github.com/your_username/SYBAU.git
cd SYBAU
mkdir build && cd build
cmake ..
make
