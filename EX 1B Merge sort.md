# EX 1B Merge Sort
## DATE: 25/08/2025
## AIM:
To write a python program to sort the first half of the list using merge sort.

## Algorithm
1. To implement the Merge Sort algorithm in Python for sorting an array of floating-point numbers entered by the user. 
2. The program uses the Divide and Conquer strategy to divide the array and then merge them in sorted order.
3. The user is prompted to input n numbers, which are stored in a Python list using append().
4. This function splits the array recursively into subarrays until single elements are left. 
5.  Merges two sorted halves by comparing elements from left (L) and right (R) subarrays.
6.  The final sorted array is printed 

## Program:

### Program to implement Merge Sort
**Developed by:** SINGARAVETRIVEL S 
**Register Number:** 212222220048
```
def merge(arr, l, m, r):
    n1=m-l+1
    n2=r-m
    L=[0]*(n1)
    R=[0]*(n2)
    for i in range(0, n1):
        L[i]=arr[l + i]
 
    for j in range(0, n2):
        R[j]=arr[m + 1 + j]
    i = 0     
    j = 0     
    k = l     
    while i < n1 and j < n2:
        if L[i] <= R[j]:
            arr[k] = L[i]
            i += 1
        else:
            arr[k] = R[j]
            j += 1
        k += 1
    while i < n1:
        arr[k] = L[i]
        i += 1
        k += 1
    while j < n2:
        arr[k] = R[j]
        j += 1
        k += 1
def mergeSort(arr, l, r):
    if l < r:
        m = l+(r-l)//2
        mergeSort(arr, m+1, r)
        merge(arr, l, m, r)
arr =[] 
n =int(input())
for i in range(n):
    arr.append(float(input()))
print("Given array is")
for i in range(n):
    print("%.1f" % arr[i],end=" ")
mergeSort(arr, 0, n-1)
print("\n\nSorted array is")
for i in range(n):
    print("%.1f" % arr[i],end=" ")
```
## Output:
![Screenshot 2025-05-24 172030](https://github.com/user-attachments/assets/db6498df-4914-45b0-ac13-f202dd991555)

## Result:
The program successfully sorts the first half of the given array using merge sort. where only the first half is sorted, and the second half remains unchanged.
