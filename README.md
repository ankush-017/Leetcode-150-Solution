# LeetCode 150 Solutions 

This repository contains my solutions to the **LeetCode Top 150 Interview Questions**, implemented in **Java**.

The goal of this repository is to practice data structures and algorithms, improve problem-solving skills, and prepare for technical interviews.

---

## Contents

* Clean and optimized Java solutions
* Step-by-step logical approach
* Time & space complexity analysis
* Common interview patterns and techniques

---

## Topics Covered

* Arrays & Strings
* Two Pointers
* Sliding Window
* Stack & Queue
* Linked List
* Binary Search
* Trees & Binary Search Trees
* Graphs
* Dynamic Programming
* Greedy Algorithms
* Backtracking
* Heap / Priority Queue

---

## 🗂️ Folder Structure

```
Leetcode-150-Solution/
│
├── Arrays/
├── Strings/
├── LinkedList/
├── Stack/
├── Queue/
├── Trees/
├── Graphs/
├── DP/
├── Greedy/
└── README.md
```

---

## Example Problem

**LeetCode 150 – Evaluate Reverse Polish Notation**

* Stack-based evaluation
* Time Complexity: `O(n)`
* Space Complexity: `O(n)`

```java
class Solution {
    public int evalRPN(String[] tokens) {
        Stack<Integer> stack = new Stack<>();

        for (String token : tokens) {
            if ("+-*/".contains(token)) {
                int b = stack.pop();
                int a = stack.pop();
                switch (token) {
                    case "+": stack.push(a + b); break;
                    case "-": stack.push(a - b); break;
                    case "*": stack.push(a * b); break;
                    case "/": stack.push(a / b); break;
                }
            } else {
                stack.push(Integer.parseInt(token));
            }
        }
        return stack.pop();
    }
}
```

---

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/ankush-017/Leetcode-150-Solution.git
   ```

2. Open in your IDE (VS Code / IntelliJ)

3. Navigate to the topic folder

4. Run and test the solution

---

## 🎯 Goal

* Strengthen DSA fundamentals
* Improve coding interview confidence
* Build a clean and reusable reference

---

## ⭐ Contributions

Feel free to fork, star ⭐, or suggest improvements!

---

## 👨‍💻 Author

**Ankush Kumar**
 Aspiring Software Engineer | Java | DSA | Backend

---

Happy Coding
