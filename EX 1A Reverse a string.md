# EX 1A Reverse a String
## DATE:
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm
1. 
2. 
3. 
4.  
5.   

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
