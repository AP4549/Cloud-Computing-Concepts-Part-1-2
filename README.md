# Cloud-Computing-Concepts-Part-1-2
# Distributed Systems Projects: MP1 & MP2

## Overview
This repository contains two machine programming assignments focused on distributed systems:
- **MP1**: Membership Protocol - Implementing gossip-style/SWIM-style failure detection
- **MP2**: Distributed Key-Value Store - Building a fault-tolerant, replicated key-value store

## MP1: Membership Protocol

### Concepts
- Gossip Protocol / SWIM-style failure detection
- Completeness (all nodes detect failures)
- Accuracy (minimize false positives)
- Scalable and efficient message passing

### Running MP1
```bash
# Compile
cd MP1/
make clean
make

# Run simulation
./Application testcases/memberlist.conf

# Check logs
cat dbg.log

# Run grader
chmod +x Grader.sh
./Grader.sh
```

## MP2: Distributed Key-Value Store

### Concepts
- Replication across multiple nodes
- Quorum-based consistency
- Failure recovery and data re-replication

### Running MP2
```bash
# Compile
cd MP2/
make clean
make

# Run simulation
./Application testcases/sample.conf

# Check logs
cat dbg.log

# Run grader
chmod +x KVStoreGrader.sh
./KVStoreGrader.sh
```

## Requirements
- C++11 or later (gcc 4.7+)
- Linux/macOS environment
- `make` installed

## Submitting
```bash
python submit.py
```

## Key Takeaways
- MP1 focuses on failure detection in distributed systems
- MP2 builds on MP1 to implement a fault-tolerant key-value store
- Both projects demonstrate core distributed computing principles
