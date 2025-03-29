# Basic-Algorithms-
# Euclid's Algorithm for GCD

## 📌 Introduction
This repository contains an implementation of **Euclid's Algorithm** for finding the **Greatest Common Divisor (GCD)** of two numbers in Python.

## 📜 Algorithm Explanation
Euclid’s Algorithm is based on the principle that:
> **GCD(a, b) = GCD(b, a % b)**  
It keeps reducing the numbers using the modulus operation until one of them becomes zero.

## 📝 Code Implementation
```python
def gcd(a, b):
    while b:
        a, b = b, a % b
    return a

# Example usage
num1 = 48
num2 = 18
print(f"GCD of {num1} and {num2} is {gcd(num1, num2)}")
