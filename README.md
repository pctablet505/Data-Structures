# Data Structures

Comprehensive Python implementations of advanced data structures and algorithms, primarily from **CLRS** (*Introduction to Algorithms, 3rd Edition*) and inspired by competitive programming problems.

## Description

This repository contains clean, self-contained Python implementations of fundamental and advanced data structures. It serves as both a reference for algorithmic study and a practical library for competitive programming. Special emphasis is placed on balanced trees, range query structures, and advanced priority/search structures such as the van Emde Boas Tree.

## Implemented Data Structures

| Data Structure | File(s) | Key Operations | Notes |
|---|---|---|---|
| **AVL Tree** | `AVL Tree.py` | Insert, Delete, Search — *O(log n)* | Self-balancing BST with height factor |
| **Binary Search Tree** | `Binary Search Tree.py` | Insert, Delete, Search — *O(h)* | Standard BST implementation |
| **BST with Duplicates** | `Binary Search Tree wit Duplicate keys allowed.py` | Insert, Delete, Search | Handles duplicate keys |
| **Red-Black Tree** | `Red Black Tree.py` | Insert, Delete, Search — *O(log n)* | Balanced BST with color properties (CLRS) |
| **Splay Tree** | `Splay tree.py` | Access, Insert, Delete — amortized *O(log n)* | Self-adjusting BST |
| **Treap** | `Treap.py`, `treap1.py` | Insert, Delete, Split, Merge — *O(log n)* expected | Randomized BST + heap priority |
| **Implicit Treap** | `implicit treaps.py` | Split, Merge, Range operations — *O(log n)* expected | Sequence/range operations on array |
| **Segment Tree (RMQ)** | `Segment Tree RMQ.py` | Build, Query, Update — *O(log n)* | Range Minimum/Maximum Query |
| **Segment Tree (Point Update, Range Sum)** | `segment tree point update range query sum.py` | Point Update, Range Sum — *O(log n)* | Fenwick-tree alternative use case |
| **Sparse Table (RMQ)** | `Sparse Table RMQ.py` | Query — *O(1)*, Build — *O(n log n)* | Static range minimum query |
| **Sparse Table (Range Maximum Query)** | `Sparse Table Range Maximum Query.py` | Query — *O(1)* | Static range maximum query |
| **Sparse Table (Range Sum Query)** | `Sparse Table Range Sum Query.py` | Query — *O(1)* | Static range sum query |
| **Binary Indexed Tree (Fenwick Tree)** | `binary indexed tree.py` | Point Update, Prefix Sum — *O(log n)* | Space-efficient prefix sums |
| **Skip List** | `Skip List.py` | Search, Insert, Delete — *O(log n)* expected | Probabilistic alternative to balanced trees |
| **Disjoint Set Union (Union-Find)** | `Disjoint Set.py` | Union, Find — *O(α(n))* | Path compression + union by rank/size |
| **van Emde Boas Tree** | `van Emde Boas Tree/` | Insert, Delete, Successor, Predecessor — *O(log log U)* | `O(u)` and `O(n log log u)` space variants |
| **Stack (Array)** | `Stacks using array.py` | Push, Pop, Peek — *O(1)* | Fixed/dynamic array based |
| **Stack (Linked List)** | `Stack using linked list.py` | Push, Pop, Peek — *O(1)* | Singly linked list based |
| **Minimum Stack** | `minimum stack.py` | Push, Pop, GetMin — *O(1)* | Tracks minimum in constant time |
| **Queue (Array)** | `queue using array.py` | Enqueue, Dequeue — *O(1)* | Circular array implementation |
| **Queue (Linked List)** | `Queue using linked list.py` | Enqueue, Dequeue — *O(1)* | Linked list based |
| **Deque (Array)** | `deque using array.py` | Insert/Delete at both ends — *O(1)* amortized | Double-ended queue |
| **Deque (Doubly Linked List)** | `Deque using doubly linked list.py` | Insert/Delete at both ends — *O(1)* | DLL based |
| **Singly Linked List** | `Singly Linked List.py` | Insert, Delete, Search — *O(n)* | Classic linked list |
| **Doubly Linked List** | `Doubly linked list.py` | Insert, Delete, Search — *O(n)* | Bidirectional traversal |
| **Two Stacks in One Array** | `2 stacks in one array.py` | Push, Pop for two stacks — *O(1)* | Space-efficient stack sharing |

### van Emde Boas Tree Variants

The `van Emde Boas Tree/` directory contains multiple implementations:
- **`van Emde Boas Tree O(u) space.py`** / **`van Emde Boas Tree O(u) space new.py`**: Full array-based recursive structure using *O(u)* space.
- **`van Emde Boas Tree O(n(log(log(u)))) space .py`**: Space-optimized variant using *O(n log log u)* space.

## How to Use

Each data structure is implemented in a standalone `.py` file and can be run independently for demonstration/testing:

```bash
python "AVL Tree.py"
python "Segment Tree RMQ.py"
python "van Emde Boas Tree/van Emde Boas Tree O(u) space.py"
```

You can also import the classes/functions into your own scripts:

```python
from "AVL Tree" import AVLTree  # adjust import based on module naming
```

> **Note:** Some filenames contain spaces; for imports, consider renaming or using `importlib`.

## Project Structure

```
Data-Structures/
├── AVL Tree.py
├── Binary Search Tree.py
├── Binary Search Tree wit Duplicate keys allowed.py
├── Red Black Tree.py
├── Splay tree.py
├── Treap.py
├── treap1.py
├── implicit treaps.py
├── Segment Tree RMQ.py
├── segment tree point update range query sum.py
├── Sparse Table RMQ.py
├── Sparse Table Range Maximum Query.py
├── Sparse Table Range Sum Query.py
├── binary indexed tree.py
├── Skip List.py
├── Disjoint Set.py
├── van Emde Boas Tree/
│   ├── van Emde Boas Tree O(u) space.py
│   ├── van Emde Boas Tree O(u) space new.py
│   └── van Emde Boas Tree O(n(log(log(u)))) space .py
├── Stacks using array.py
├── Stack using linked list.py
├── minimum stack.py
├── queue using array.py
├── Queue using linked list.py
├── deque using array.py
├── Deque using doubly linked list.py
├── Singly Linked List.py
├── Doubly linked list.py
└── 2 stacks in one array.py
```

## References

- **CLRS** — *Introduction to Algorithms*, 3rd Edition. Cormen, Leiserson, Rivest, Stein.
- Competitive Programming resources and problem sets for practical applications.
