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
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: jagadeeshreddy
RegisterNumber: 22001910
'''
def selection_sort(list_of_nums):
    n = len(list_of_nums)
    for i in range(n):
        min_idx = i
        for j in range(i+1, n):
            if list_of_nums[min_idx] > list_of_nums[j]:
                min_idx = j
        list_of_nums[i], list_of_nums[min_idx] = list_of_nums[min_idx], list_of_nums[i]
    return list_of_nums
list_of_nums = eval(input())
print(selection_sort(list_of_nums))
```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: jagadeeshreddy
RegisterNumber: 22001910
'''
def insertion_sort(nums):
    for i in range(1, len(list)):
        currentvalue = list[i]
        position = i 
        
        while position > 0 and list[position - 1] > currentvalue:
            list[position] = list[position - 1]
            position = position - 1
            
        list[position] = currentvalue 
        
list = eval(input())
insertion_sort(list)
print(list)
```

## Output:
![Screenshot (23)](https://user-images.githubusercontent.com/120623104/214884768-7e56270d-66a0-4788-aa97-113a3deade0f.png)
![Screenshot (24)](https://user-images.githubusercontent.com/120623104/214884954-f3a2d274-5af4-416e-aee7-ad1a9ba9e462.png)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
