# Architecture

## Overview

This project implements a single-instrument Limit Order Book using
Price-Time priority.

## Main Components

### Order

Represents a single limit order.

### PriceLevel

Stores orders at the same price using FIFO ordering.

### LimitOrderBook

Maintains bid and ask price levels and performs order matching.

### MemoryPool

Provides pre-allocated storage for orders to avoid dynamic memory
allocation in the hot path.

## Planned Data Structures

- Ordered price levels
- Intrusive doubly linked lists for orders at the same price
- Flat lookup table for Order ID lookup
- Pre-allocated memory pool

## Performance Goals

- Correct Price-Time matching
- O(1) Order ID lookup
- O(1) order cancellation
- Zero allocations in the hot path
- Sub-microsecond target latency for critical operations
- At least 1 million events per second as an initial target
