# EXPERIMENT 1 - INTRODUCTION TO PYTHON PROGRAMMING

This repository contains Python scripts created to address various problems in ECE2112. A summary of each script is provided below.

# Table of Contents
- [Introduction](#introduction)
- [Alphabet Soup Problem](#alphabet-soup-problem)
- [Emoticon Problem](#emoticon-problem)
- [Unpacking list Problem](#unpacking-list-problem)

---

## Introduction
This repository contains Python scripts developed for EXPERIMENT 1 - Introduction to Python Programming, focused on solving basic programming problems using fundamental Python functions. The main objective of the experiment is to enable students to:

###### 1. Identify and understand basic codes and functions in Python.
###### 2. Apply these codes and functions in creating simple Python programs.

--- 


### 1. Alphabet Soup Problem

###### Create a function that takes a string and returns a string with its letters in alphabetical order.


**Function:**

```python

def sort_string_alphabetically():
    # Get a string from the user
    user_string = input("enter a string: ")
    
    # Arrange the characters in alphabetical order
    sorted_string = ''.join(sorted(user_string))
    
    return sorted_string

# Example of how to use the function:
result = sort_string_alphabetically()
print("Output:", result)

```
**Output:**

<img width="348" height="61" alt="Screen Shot 2025-08-25 at 12 10 50 PM" src="https://github.com/user-attachments/assets/b511a7d5-fd02-47a6-91ee-7d09c7256888" />


### 2. Emoticon Problem

###### Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad, and mad with their corresponding emoticon:

**Function:**

```python

def main():
    # Get user input
    sentence = input("Enter a sentence: ")
    
    # Convert words
    sentence = convert(sentence)
    
    # Print converted
    print("Output sentence:", sentence)

def convert(sentence):
    # Replace words with emoticons
    sentence = sentence.replace("smile", ":)")
    sentence = sentence.replace("grin", ":D")
    sentence = sentence.replace("sad", ":(")
    sentence = sentence.replace("mad", ">:(")
    
    # Return modified sentence
    return sentence

# Start program
main()

```

**Output:**

<img width="254" height="59" alt="Screen Shot 2025-08-25 at 12 13 07 PM" src="https://github.com/user-attachments/assets/d073f3b7-24a3-46ef-9b68-1d8249eddfa5" />


### 3. Unpacking list Problem

###### Unpack the list, write your code here into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.

**Function:** 

```python
def unpack_and_display():
    user_input = input("Please provide a list of items: ")
    items = user_input.split()
    
    first_item, *middle_items, last_item = items
    
    print("First item:", first_item)
    print("Middle items:", middle_items)
    print("Last item:", last_item)

unpack_and_display()

```

**Output:**

<img width="476" height="91" alt="Screen Shot 2025-08-25 at 12 16 26 PM" src="https://github.com/user-attachments/assets/b02a3aea-7510-4904-87b2-7f803a9fb194" />





