# push_swap

This project is an introduction to **linked list management** and basic **algorithm optimization**.

The purpose of this project is to sort a list of integers using **two stacks**, **stack A** and **stack B**, implemented with **linked lists**, and a **limited** set of stack manipulation instructions. The goal is to **sort** the numbers using the **minimum** number of operations possible.

First, the numbers to sort are passed as arguments to the program. The program then verifies that all arguments are **valid numbers**. Once validated, the numbers are pushed into **stack A** before applying the **sorting algorithm**.  

This project uses a **sorting algorithm** that manipulates **stack A** and **stack B** using a **radix-based** approach. Once the numbers are sorted in **stack A**, the program ends its execution.

## The new topics in this project
Linked lists

- **Linked** lists are **data structures** that contain a **value** and a **pointer** to the next node in the list.

- They are useful for storing data because adding a new element only requires creating a **new node** and linking it to the **existing list**.

Sorting algorithm 
- In this project, you are free to use the algorithm of your choice, as long as it is **sufficiently optimized** to **sort** the numbers with a limited number of operations.

- This implementation uses the **radix algorithm**. **Radix sort** is explained in more detail in the *“How the program works”* section. In short, it is an algorithm based on the binary representation of numbers.

## How the program works
1. All numbers passed as arguments are first combined into a single string using the `ft_strjoin()` function from the `libft` project. This allows the program to handle inputs such as:
`./push_swap 1 2 "3 4" 5.`

2. The combined string is then split using the `ft_split()` function, ensuring that numbers passed together **(like "3 4")** are processed as separate values.

3. All numbers are **parsed** and **validated**, and **stack A** is initialized with these values.

4. The **radix algorithm** is applied using stack manipulation instructions and **stack B** to progressively sort the values in **stack A**.

5. **Radix sort** works by sorting numbers digit by digit, from the least significant digit to the most significant digit. In this project, the algorithm is applied using the **binary** representation of the numbers.

6. Once **stack A is fully sorted**, the program finishes execution.

## Installation
- Run make
- Execute the program with the arguments of your choice

```bash
  make
  ./push_swap [number_of_your_choice]
```
    
<div>
    <h3>Language & Tool</h3>
    <p>
        <img src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white"/>
        <img src="https://img.shields.io/badge/Make-427819?style=for-the-badge&logo=gnu&logoColor=white"/>
    </p>
</div>
