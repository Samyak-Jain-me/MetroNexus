# 📚 Project Requirements

---

## 🟡 Section 1: Java Users — Java Collections Framework

The **Java Collections Framework** provides a standard architecture to store and manipulate groups of objects using interfaces and classes such as `ArrayList`, `LinkedList`, `HashMap`, and `Stack`.

![Flowchart](https://user-images.githubusercontent.com/71463658/101475597-9db6f400-3972-11eb-8b9f-dec58a00104f.png)

---

### 🧩 Collections Used in This Project

#### 📁 `Graph_M.java`
- `ArrayList` — For adjacency lists and dynamic array usage.
- `LinkedList` — For queue-based traversal.
- `Stack` — For DFS and backtracking.
- `HashMap` — For mapping nodes to neighbors.

#### 📁 `Heap.java`
- `ArrayList` — Represents the heap.
- `HashMap` — Maps values to indices for O(1) access and updates.

---

### 🗂️ Data Structures Overview

| Data Structure | Java Class Used       | Purpose                                                                 |
|----------------|------------------------|-------------------------------------------------------------------------|
| Array          | `ArrayList`            | Resizable array with index-based access                                |
| Hash Map       | `HashMap`              | Stores key–value pairs with O(1) average access                         |
| Linked List    | `LinkedList`           | Efficient insertions/deletions during traversal                        |
| Stack          | `Stack` / `LinkedList` | LIFO structure used in DFS and recursion emulation                     |
| Heap           | `ArrayList + HashMap`  | Implements Min/Max heap using tree-based logic                         |
| Graph          | `ArrayList + HashMap`  | Stores nodes and edges using adjacency list                            |

---

## 🔵 Section 2: C++ Users — STL (Standard Template Library)

For C++ developers, the project logic can be translated using equivalent STL containers that serve the same purpose as Java collections.

---

### 🧩 STL Containers for This Project

#### 📁 `Graph.cpp` (Equivalent to `Graph_M.java`)
- `vector` — For adjacency lists and resizable arrays.
- `list` — For BFS/DFS traversal queues.
- `stack` — To implement DFS/backtracking.
- `unordered_map` — Maps nodes to neighbors.

#### 📁 `Heap.cpp` (Equivalent to `Heap.java`)
- `vector` — Used as the underlying structure for heaps.
- `unordered_map` — Stores value–index pairs for quick access.

---

### 🗂️ Data Structures Overview

| Data Structure | C++ STL Used            | Purpose                                                                 |
|----------------|--------------------------|-------------------------------------------------------------------------|
| Array          | `vector`                 | Resizable dynamic array with fast index access                         |
| Hash Map       | `unordered_map`          | Stores key–value pairs, average O(1) access                            |
| Linked List    | `list`                   | Doubly linked list, ideal for traversal and queue ops                  |
| Stack          | `stack`                  | LIFO structure used for DFS and recursion logic                        |
| Heap           | `priority_queue + map`   | Min/Max heap using `priority_queue`; track indices with `map` if needed|
| Graph          | `vector + unordered_map` | Adjacency list representation of graph                                 |

---

### 🔄 Cross-Reference Table (Java ↔️ C++)

| Concept          | Java Class     | C++ STL Equivalent   |
|------------------|----------------|-----------------------|
| Dynamic Array     | `ArrayList`    | `vector`              |
| Hash Map          | `HashMap`      | `unordered_map`       |
| Linked List       | `LinkedList`   | `list`                |
| Stack             | `Stack`        | `stack`               |
| Heap              | `ArrayList` + `HashMap` | `priority_queue` + `unordered_map` |
| Graph (Adj. List) | `ArrayList` + `HashMap` | `vector` + `unordered_map` |

---

📌 **Note for C++ Users:**  
If you're implementing a heap that needs frequent index updates (like Dijkstra’s priority updates), you may use a custom heap implementation using `vector` and `unordered_map` for efficiency.

