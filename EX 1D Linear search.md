# EX 1D Linear search
## DATE: 25/08/2025
## AIM:
To write a python program for a search function with parameter list name and the value to be searched using string values.

## Algorithm
1. Start by reading the number of elements and storing them in a list.
2. Accept the search element n from the user.
3. Traverse the list using a loop to compare each element with n.
4. If a match is found, return True; otherwise, return False after the loop.
5. Print "Found" if True, else print "Not Found". 

## Program:

### Program to implement a search function with parameter list name and the value to be searched using string values.
**Developed by:** SINGARAVETRIVEL S
**Register Number:** 212222220048
```
def search(List,n):
    for i in range(len(List)):
        if List[i]==n:
            return True
    return False
    
List=[]
x=int(input())
for i in range(x):
    List.append(input())
n=input()
search(List,n)
if search(List,n)==True:
    print("Found")
else:
    print("Not Found")
```
## Output:
![Screenshot 2025-05-24 173536](https://github.com/user-attachments/assets/165cf6fd-07c4-49e9-8ad6-b048d173ac5d)

## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
