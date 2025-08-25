# EX 1C Quick Sort
## DATE: 25/08/2025
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
1. Select the last element as the pivot and partition the array around it.
2. Place elements smaller than the pivot to its left and larger to its right.
3. Recursively apply Quick Sort to the left sub-array before the pivot.
4. Recursively apply Quick Sort to the right sub-array after the pivot. 
5. Repeat until the entire array is sorted and then print the sorted array.   

## Program:

### Program to implement implement quick sort using the last element as pivot on the list of float values.
**Developed by:** SINGARAVETRIVEL S
**Register Number:** 212222220048
```
def fun(arr,low,high):
    pivot=arr[high]
    i=low-1
    for j in range(low,high):
        if arr[j]<pivot:
            i += 1
            arr[i],arr[j]=arr[j],arr[i]
    arr[i+1],arr[high]=arr[high],arr[i+1]
    return i+1
def quickSort(arr,low,high):
    if low<high:
        pi=fun(arr,low,high)
        quickSort(arr,low,pi-1)
        quickSort(arr,pi+1,high)
n=int(input())
arr=[]
for i in range(n):
     arr.append(float(input())) 
quickSort(arr,0,len(arr)-1)
print("Sorted array is:")
for i in range(n):
    print("%.1f" %arr[i])
```
## Output:
![Screenshot 2025-05-24 172715](https://github.com/user-attachments/assets/b78926e9-edd1-41f3-9f5e-96669af82150)

## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
