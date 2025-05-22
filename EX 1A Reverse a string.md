# EX 1A Reverse a String
## DATE:
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm
1. Define a recursive function reverse_string(s): This function will take a string s as input and reverse it.
2. Handle the base case: If the string s is empty, return s itself (as an empty string is its own reverse).
3. Perform recursive step: Otherwise, take the last character of s (s[-1]) and concatenate it with the result of calling reverse_string on the rest of the string (s[:-1]).
4. Get user input: Prompt the user to enter a string and store it in the variable s.
5. Print the reversed string: Call reverse_string(s) with the user's input and print the returned reversed string. 

## Program:
### Program to implement Reverse a String
### Developed by: NARASIMHAN S
### Register Number: 212223230133 
```
def reverse_string(s):
    if len(s) == 0:
        return s
    return s[-1] + reverse_string(s[:-1])

s = input() 
print(reverse_string(s))
```

## Output:
![image](https://github.com/user-attachments/assets/cd044439-4c1d-402a-a6cd-e53d7b0657c8)


## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
