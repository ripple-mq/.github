# Ripple

**Ripple** is a high-performance, distributed, in-memory event streaming system written in Go. Designed for scalability and fault tolerance, Ripple provides low-latency data streaming with support for replication, replay, leader election, and high-throughput consumer access.

---

## 🚀 Key Features

- **Distributed Architecture**: Built for horizontal scalability with replication and leader election.
- **In-Memory Streaming**: Ultra-low latency event streaming, optimized for speed.
- **Non-Blocking IO**: Uses native OS-level IO multiplexing (`epoll` on Linux, `kqueue` on BSD/Unix).
- **Fault Tolerant**: Automatically detects node failures and re-elects leaders.
- **Replay & Persistence**: Events can be replayed for analytics or recovery.
- **Replication**: Asynchronous dumping to read replicas.
- **Acknowledgment Levels**: Supports various consumer acknowledgment modes.
- **Load Balancing**: Intelligent routing for reading and writing across nodes.
- **gRPC API**: High-performance RPC for communication.
- **ZooKeeper Coordination**: Leader election, metadata management, and cluster coordination.

---

## 🧱 Core Components

### 🔹 ripple-server
The core server that handles incoming events, maintains in-memory queues, manages replication, and interfaces with ZooKeeper.

### 🔹 go-client
A Go client SDK for producing and consuming events from Ripple clusters.

### 🔹 benchmark
Performance benchmarking tools to evaluate Ripple’s throughput and latency under different scenarios.

