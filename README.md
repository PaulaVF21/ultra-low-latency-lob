# Ultra-Low-Latency Limit Order Book

A deterministic Limit Order Book and matching engine implemented in C++20,
focused on low latency, predictable performance and cache-efficient data structures.

## Goals

- Price-Time priority matching
- O(1) order lookup and cancellation
- Zero dynamic allocations in the hot path
- Cache-efficient memory layout
- Unit testing with Google Test
- Performance benchmarking with Google Benchmark
- Synthetic and real market data replay

## Tech Stack

- C++20
- CMake
- GCC / Clang
- Google Test
- Google Benchmark
- Linux
- GitHub Actions
