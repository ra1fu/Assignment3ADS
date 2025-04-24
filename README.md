# Assignment3ADS
# Assignment 3 — Algorithms and Data Structures

This project implements two core data structures from scratch:

1. **MyHashTable<K, V>** — a custom hash table with separate chaining and dynamic resizing
2. **BST<K, V>** — a binary search tree implemented **without recursion**, including in-order traversal using an iterator

---

## Part 1: MyHashTable<K, V>

### Features:
- Internal `HashNode<K, V>` class (private)
- `put(K key, V value)` — insert or update
- `get(K key)` — fetch value by key
- `remove(K key)` — delete entry by key
- `contains(V value)` — check for a value
- `getKey(V value)` — find key by value
- **Automatic resize** when load factor exceeds 0.75

### Testing:
Implemented in `TestHashTable.java`:
- Inserts 10,000 random entries using a custom `MyTestingClass` as key
- Verifies access through `get()`
- Prints number of found entries

---

## Part 2: BST<K, V>

### Features:
- `put(K key, V value)` — iterative insertion
- `get(K key)` — iterative search
- `delete(K key)` — iterative removal
- `size()` — returns number of elements
- `iterator()` — in-order traversal **without recursion**
- `Entry<K, V>` — provides access to key and value in traversal

### Testing:
Implemented in `TestBST.java`:
- Inserts sample nodes into the tree
- Prints all elements using the iterator
- Demonstrates deletion and size update

---

## How to Run

Compile and run test files from the `test` package:
```bash
javac models/*.java test/*.java
java test.TestHashTable
java test.TestBST
