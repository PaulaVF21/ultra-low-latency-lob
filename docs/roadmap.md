# Development Roadmap

## Phase 0 - Project Setup

- [ ] Configure CMake
- [ ] Configure compiler warnings
- [ ] Integrate Google Test
- [ ] Integrate Google Benchmark

## Phase 1 - Core Data Structures

- [ ] Define Side
- [ ] Implement Order
- [ ] Implement PriceLevel
- [ ] Implement LimitOrderBook

## Phase 2 - Matching Engine

- [ ] Add orders
- [ ] Implement Price-Time priority
- [ ] Handle full fills
- [ ] Handle partial fills
- [ ] Cancel orders

## Phase 3 - Memory Management

- [ ] Implement MemoryPool
- [ ] Implement flat Order ID lookup
- [ ] Remove allocations from the hot path

## Phase 4 - Testing

- [ ] Unit tests
- [ ] AddressSanitizer
- [ ] UndefinedBehaviorSanitizer

## Phase 5 - Performance

- [ ] Google Benchmark
- [ ] Cachegrind
- [ ] perf
- [ ] Compare baseline and optimized implementations

## Phase 6 - Market Data

- [ ] Synthetic order generator
- [ ] Market data parser
- [ ] Real market data replay
