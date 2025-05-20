# EX 1D Linear search
## DATE:
## AIM:
To Write a python program to implement the binary search on the given list of characters.

## Algorithm
1. Initialize pointers: Set low = 0 and high = len(list) - 1.
2. Repeat until found or exhausted: While low <= high, find the middle index using mid = (low + high) // 2.
3. If list[mid] == target, return the index.
4. If list[mid] < target, search in the right half (low = mid + 1). Else, search in the left half (high = mid - 1).
5. Element not found: If loop ends, the character is not in the list.   

## Program:
### Developed by: NARASIMHAN S
### Register Number: 212223230133
```
def binarySearchAppr(a,st,en,x):
    while st<=en:
        mid=(st+en)//2
        if a[mid]==x:
            print("Element is present at index",mid)
            break
        elif x<a[mid]:
            en=mid-1
        elif x>a[mid]:
            st=mid+1
    else:
        print("Element is not present")
arr=[input() for _ in range(int(input()))]
x=input()
arr.sort()
```

## Output:

![image](https://github.com/user-attachments/assets/7c5c4970-1fb4-4337-b35c-6d659b3aea69)

## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, print the index position.
