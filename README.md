# EXPERIMENT 1 - INTRODUCTION TO PYTHON PROGRAMMING

This repository contains Python scripts created to address various problems in ECE2112. A summary of each script is provided below.

# Table of Contents
- [Introduction](#introduction)
- [Alphabet Soup Problem](#alphabet-soup-problem)
- [Emoticon Problem](#emoticon-problem)

---

## Introduction
This repository contains Python scripts developed for EXPERIMENT 1 - Introduction to Python Programming, focused on solving basic programming problems using fundamental Python functions. The main objective of the experiment is to enable students to:

###### 1. Identify and understand basic codes and functions in Python.
###### 2. Apply these codes and functions in creating simple Python programs.

--- 


### 1. Normalization Problem

###### A randomly generated 5x5 array is required to be normalized for this task. To normalize the random array, first produce it, then center it by subtracting the mean, then scale it by dividing it by the standard deviation. Save the normalized array to a file named `X_normalized.npy}.


**Function:**

```python

import numpy as np

# Create a 5x5 random values
X = np.random.random((5, 5))

# Calculate the mean and standard deviation
X_mean = np.mean(X)
X_std = np.std(X)

# Standardize the matrix
X_normalized = (X - X_mean) / X_std

# Save the standardized matrix
np.save('X_normalized.npy', X_normalized)

# Load and display the saved data
print("\nOriginal Array:\n", X)
print("\nNormalized Array:\n", X_normalized)

```
**Output:**

<img width="582" height="261" alt="image" src="https://github.com/user-attachments/assets/2bdfd781-cfb4-4947-99d2-fd617fa31c8c" />


### 2. Divisible by 3 Problem

###### The task is to create a 10x10 array containing the squares of the initial 100 positive integers. Finding every element in the array divisible by three is the aim, and the elements saved in a file named `div_by_3.npy` are the result.


**Function:**

```python

import numpy as np

# Generate random positive integer from 1 to 100
squares = np.arange(1, 101)**2

# Reshape into a 10x10 matrix
squares_10x10 = squares.reshape(10, 10)

# Extract elements divisible by 3
div_by_3 = squares_10x10[squares_10x10 % 3 == 0]

# Save the result to a file
np.save('div_by_3.npy', div_by_3)

# Load and display the saved data
data = np.load('div_by_3.npy')
data

```

**Output:**

<img width="631" height="119" alt="image" src="https://github.com/user-attachments/assets/808d9231-857b-43b6-84db-51b2803995eb" />







