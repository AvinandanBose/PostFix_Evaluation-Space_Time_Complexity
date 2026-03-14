# Postfix Evaluation: Space & Time Complexity Analysis

![GitHub repo size](https://img.shields.io/github/repo-size/AvinandanBose/PostFix_Evaluation-Space_Time_Complexity)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

## 📌 About The Repository
This repository provides a deep dive into **Postfix Evaluation**, detailing how it works under the hood at both the programmed and hardware levels. It includes detailed PDF notes focusing on memory mechanisms, hardware instructions, and comprehensive space and time complexity analyses.

## 📂 Topics & Resources Included

The repository contains several carefully detailed PDF documents explaining the following concepts:

* **Postfix Evaluation Concepts:** Core evaluation mechanisms and walkthroughs.
* **PUSH Mechanism:** Hardware memory mechanism behind pushing to a stack.
* **Operation Mechanism:** How operations are processed in hardware memory.
* **POP Instructions:** Logical (Programmed) POP vs. Hardware Instruction POP.
* **Array Address Calculation:** Hardware mechanism for `BaseAddress + index × SizeOf(DataType)`.
* **[Extra] ENDL and ASCII:** Hardware mechanisms related to end-line characters and ASCII.
* **Complexity Analysis:** Detailed breakdown of Space and Time complexities for Postfix operations.

## ⏱️ Complexity Analysis Summary

In Postfix Evaluation, the conversion from infix to postfix remains the same standard process. For evaluating a postfix expression (e.g., converted from `(a + b)^(c - d)/e`), the complexities are as follows:

### Time Complexity: `O(n)`
* Basic operations like multiplication, division, exponentiation, and modulo take constant time: **`O(1)`** per operation.
* Each character/token in the expression is processed sequentially. Using a switch-case implementation, each case executes in **`O(1)`** time.
* Pushing and popping from the stack take **`O(1)`** time.
* Traversing the entire expression of length `n` requires visiting each element once.
* **Total Time Complexity = `O(1) + O(n) + O(1) + O(n-1) = O(n)`**, where `n` is the length of the postfix string.

### Space Complexity: `O(n)`
* In the worst-case scenario, pushing operands to the stack takes **`O(n)`** space.
* **Total Space Complexity = `O(n)`**, scaling linearly with the number of operands in the expression.

## 💻 Code Implementation

Looking for the actual code? The C++ implementation of Postfix Evaluation can be found in the following repository:
👉 **[C++ - Data Structures Repository](https://github.com/AvinandanBose/CPLUSPLUS_DataStructure)**

## 📜 License
This repository is licensed under the [MIT License](LICENSE).




