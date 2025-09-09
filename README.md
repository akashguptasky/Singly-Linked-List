# 🌟 Singly Linked List in JavaScript

![GitHub](https://img.shields.io/badge/JavaScript-ES6-yellow)
![GitHub repo size](https://img.shields.io/github/repo-size/yourusername/linked-list-js)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains a **singly linked list implementation in JavaScript**.  
It’s perfect for beginners who want to learn **linked list data structures** and practice coding in **pure JS**.

---

## 🚀 Features

- Add a node at the **beginning**: `addFirst(data)`  
- Add a node at the **end**: `addLast(data)`  
- Remove the **first node**: `removeFirst()`  
- Remove the **last node**: `removeLast()`  
- Get the **size** of the list: `size()`  
- Print the **entire linked list**: `printList()`  

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
const LinkedList = require('./linkedList'); // or include linkedList.js

let list = new LinkedList();

list.addFirst(10);
list.addFirst(20);
list.addFirst(30);
list.addLast(40);

list.printList();  // Output: 30 -> 20 -> 10 -> 40 -> null
console.log("Size:", list.size()); // Output: 4

list.removeFirst();
list.printList();  // Output: 20 -> 10 -> 40 -> null

list.removeLast();
list.printList();  // Output: 20 -> 10 -> null
```
---
## 🎯 Learning Notes

- ✅ Understand dynamic memory allocation using this in JS classes.
- ✅ Learn pointer-based traversal for operations like add/remove.
- ✅ Practice edge cases: empty list, single-node list, multiple nodes.
- ✅ Reinforce object-oriented JS using Node and LinkedList classes.
 

```rust
Head -> Node1 -> Node2 -> Node3 -> ... -> null
```
---

## 🛠️ Tech Stack
- JavaScript (ES6)
- Node.js (optional for running)
- VS Code / any editor

## 📜 License
- This project is licensed under the MIT License.
