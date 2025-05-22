# EX 1C Quick Sort
## DATE:
## AIM:
To Write a python to implement Quick sort using the first element as pivot value

## Algorithm
1. Select the first element of the list as the pivot.
2. Partition list: Divide remaining elements into two sublists:
3. Recursively sort: Apply Quick Sort to both sublists.
4. Combine results: Concatenate the sorted left sublist, the pivot, and the sorted right sublist.
5. Base case: If the list has 0 or 1 elements, return it (already sorted).  

## Program:
### Program to implement implement quick sort using the last element as pivot on the list of float values.
### Developed by: NARASIMHAN S
### Register Number: 212223230133
```python
def quick_sort_random(a,st,en):
    if en-st>1:
        p=partition(a,st,en)
        quick_sort_random(a,st,p)
        quick_sort_random(a,p+1,en)
def partition(a,st,en):
    pivot=a[st]
    i=st+1
    j=en-1
    print("Pivot: ",pivot)
    while True:
        while(i<=j and a[i]<=pivot):
            i=i+1
        while(i<=j and a[j]>=pivot):
            j=j-1
        if i<=j:
            a[i],a[j]=a[j],a[i]
        else:
            a[st],a[j]=a[j],a[st]
            return j
nums = []
n=int(input())
for i in range(n):
    nums.append(eval(input()))
new=[]
for i in nums:
    new.append(int(i))
quick_sort_random(new, 0, len(new))
print("Sorted array:",new)

```

## Output:

![image](https://github.com/user-attachments/assets/0bf205a1-e624-42e2-97bf-dbf71ddd3aae)

## Result:
The program successfully sorts the input array using the QuickSort algorithm for the first element as pivot value.
