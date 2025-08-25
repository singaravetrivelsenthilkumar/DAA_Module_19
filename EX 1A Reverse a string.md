# EX 1A Reverse a String
## DATE:25/08/2025
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm
1. To write a Python program that takes a string input from the user and outputs the reversed version of that string.
2. The program takes a string as input using the input() function. 
3. A function named rev is defined to take one argument a.
4. The slicing syntax [::-1] is used to reverse the input string efficiently. 
5. The rev function is called with a as the argument, and the result is printed using print(). 

## Program:
### Program to implement Reverse a String  
**Developed by:** SINGARAVETRIVEL S   
**Register Number:** 212222220048

```
def rev(a):
    return a[::-1]
a=input()

print(rev(a))

```
## Output:
![Screenshot 2025-05-24 170609](https://github.com/user-attachments/assets/3b508122-9622-4864-a78b-55d7ad445898)

## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
