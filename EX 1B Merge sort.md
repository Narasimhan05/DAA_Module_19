# EX 1B Merge Sort
## DATE: 
## AIM:
To write a python program to implement merge sort using iterative approach on the given list of  float values.

## Algorithm

1. Initialize subarray size: Start with curr_size = 1 (size of subarrays to be merged).
2. Iterate through the list: Use a loop to double curr_size each time (1, 2, 4, 8,...) until it’s greater than the list length.
3. Merge subarrays: For each pair of subarrays in the list, perform a merge operation manually (like in merge sort) using indices.
4. Repeat until sorted: Continue merging larger subarrays until the entire list is sorted.  
5. Ensure the merge operation correctly handles cases where the subarray at the end has fewer elements than curr_size  

## Program:
### Program to implement Merge Sort
### Developed by: NARASIMHAN S 
### Register Number: 212223230133

```
def Merge_Sort(inp_arr):
    if len(inp_arr)>1:
        mid = 0 + len(inp_arr) // 2
        L = inp_arr[:mid]
        R = inp_arr[mid:]
        Merge_Sort(L)
        Merge_Sort(R)
        i = j = k =0
        while i <len(L) and j <len(R):
            if L[i] < R[j]:
                inp_arr[k] = L[i]
                i +=1
            else:
                inp_arr[k] = R[j]
                j +=1
            k +=1
        while i <len(L):
            inp_arr[k] = L[i]
            i += 1
            k +=1
        while j < len(R):
            inp_arr[k] = R[j]
            j +=1
            k +=1
    
n = int(input())
S= []
for i in range(n):
    S +=[float(input()),]
print("The Original array is: ",S)
Merge_Sort(S)
print("Array after sorting is: ",S)

```

## Output:
![image](https://github.com/user-attachments/assets/7d7df2ff-75d6-425c-a1d7-ed1f5dca3209)

## Result:
The program successfully merge sort using iterative approach on the given list of float values.
