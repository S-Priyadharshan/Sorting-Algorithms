# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
"""
Description: Program to sort elements in a list using Selection sort algorithm
Developed By: Priyadharshan S
Reference No.: 212223240127
"""
list1 = eval(input())
n = len(list1)
for i in range(n):
    min_idx = i
    for j in range(i + 1, n):
        if list1[j] < list1[min_idx]:
            min_idx = j
    list1[i], list1[min_idx] = list1[min_idx], list1[i]

print(list1)

```
ii)	#Insertion Sort
```
"""
Description: Program to sort elements in a list using Insertion Sort algorithm
Developed By: Priyadharshan S
Reference No.: 212223240127
"""
list1=eval(input())
n=len(list1)
for i in range(n):
    key=list1[i]
    j=i-1
    while j>=0 and key<list1[j]:
        list1[j+1]=list1[j]
        j-=1
    list1[j+1]=key
print(list1)

```

## Output:

![image](https://github.com/S-Priyadharshan/Sorting-Algorithms/assets/145854138/bfee87e4-ddca-47f9-9498-075e197605bd)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
