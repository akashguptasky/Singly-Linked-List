# 🌟 Singly Linked List in JavaScript (Fully Functional)

![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![GitHub repo size](https://img.shields.io/github/repo-size/yourusername/linked-list-js)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains a **fully functional singly linked list implementation in JavaScript**.  
It includes all **essential operations** like insertion, deletion, search, reverse, loop detection, and more.  
Perfect for beginners and intermediate learners to understand **linked lists** and practice **object-oriented JavaScript**.

---

## 🚀 Features

| Method | Description |
|--------|-------------|
| `addFirst(data)` | Add a node at the **beginning** of the list. |
| `addLast(data)` | Add a node at the **end** of the list. |
| `insertAt(index, data)` | Insert a node at a **specific position** (0-based index). |
| `removeFirst()` | Remove the **first node** from the list. |
| `removeLast()` | Remove the **last node** from the list. |
| `removeAt(index)` | Remove a node at a **specific index**. |
| `search(value)` | Search for a **value** in the list. |
| `reverse()` | Reverse the linked list **in-place**. |
| `getMiddle()` | Get the **middle node** of the linked list. |
| `detectLoop()` | Detect if the linked list contains a **cycle/loop**. |
| `size()` | Return the **number of nodes** in the list. |
| `printList()` | Print the **entire linked list** in a readable format. |

---

## 📝 Node Structure

Each node has two properties:

| Property | Description |
|----------|-------------|
| `data`   | The value stored in the node |
| `next`   | Pointer to the **next node** (null if last node) |

---

## 💻 Example Usage

```javascript
// Include your LinkedList class file
// const LinkedList = require('./linkedList');

let list = new LinkedList();

// Add nodes
list.addFirst(10);
list.addFirst(20);
list.addLast(30);
list.addLast(40);

list.printList();  
// Output: 20 -> 10 -> 30 -> 40 -> null

// Insert at index
list.insertAt(2, 25); 
list.printList();  
// Output: 20 -> 10 -> 25 -> 30 -> 40 -> null

// Remove nodes
list.removeFirst();
list.printList();  
// Output: 10 -> 25 -> 30 -> 40 -> null

list.removeLast();
list.printList();  
// Output: 10 -> 25 -> 30 -> null

list.removeAt(1);
list.printList();  
// Output: 10 -> 30 -> null

// Search
list.search(30);  // Output: Value Exists in the List
list.search(50);  // Output: Value doesn't exist

// Reverse the list
list.reverse();
list.printList();  
// Output: 30 -> 10 -> null

// Get middle node
list.getMiddle(); // Output: Middle node: 30

// Detect loop
console.log(list.detectLoop()); // Output: false

// Size of the list
console.log("Size:", list.size()); // Output: 2
```
---
## 🎯 Learning Notes

- ✅ Understand dynamic memory allocation using this in JS classes.
- ✅ Learn pointer-based traversal for operations like add/remove.
- ✅ Practice edge cases: empty list, single-node list, multiple nodes.
- ✅ Reinforce object-oriented JS using Node and LinkedList classes.
 
## Conceptual visualization:
```rust
Head -> Node1 -> Node2 -> Node3 -> ... -> null
```
---

---
## 🎨 Function Visualizations
-1️⃣ addFirst(data)
```rust
Before: Head -> 10 -> 20 -> null
addFirst(5)
After:  Head -> 5 -> 10 -> 20 -> null

```
-2️⃣ addLast(data)
```rust
Before: Head -> 5 -> 10 -> null
addLast(20)
After:  Head -> 5 -> 10 -> 20 -> null

```

-3️⃣ insertAt(index, data)
```rust
Before: Head -> 5 -> 10 -> 20 -> null
insertAt(1, 15)
After:  Head -> 5 -> 15 -> 10 -> 20 -> null

```
-4️⃣ removeFirst()
```rust
Before: Head -> 5 -> 15 -> 10 -> null
removeFirst()
After:  Head -> 15 -> 10 -> null

```

-5️⃣ removeLast()
```rust
Before: Head -> 15 -> 10 -> 20 -> null
removeLast()
After:  Head -> 15 -> 10 -> null

```

-6️⃣ removeAt(index)
```rust
Before: Head -> 15 -> 10 -> 20 -> null
removeAt(1)
After:  Head -> 15 -> 20 -> null

```

-7️⃣ search(value)
```rust
List: Head -> 15 -> 20 -> 30 -> null
search(20) -> Found
search(50) -> Not Found

```

-8️⃣ reverse()
```rust
Before: Head -> 15 -> 20 -> 30 -> null
reverse()
After:  Head -> 30 -> 20 -> 15 -> null

```

-9️⃣ getMiddle()
```rust
Head -> 10 -> 20 -> 30 -> 40 -> null
Middle: 20 (2nd node in even-length list can also be considered middle)

```
-🔟 detectLoop()
```rust
Head -> 10 -> 20 -> 30
             ^     |
             |_____|
detectLoop() -> true

```

-1️⃣1️⃣ size()
```rust
List: Head -> 10 -> 20 -> 30 -> null
size() -> 3

```
-1️⃣2️⃣ printList()
```rust
List: Head -> 10 -> 20 -> 30 -> null
Output: 10 -> 20 -> 30 -> null

```
---

## 🛠️ Tech Stack
- JavaScript (ES6)
- Node.js (optional for running)
- VS Code / any editor

## 📜 License
- This project is licensed under the MIT License.

