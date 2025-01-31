
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
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: your name:Narendran.K
RegisterNumber: 23013500
def selection_sort(nums):
    for i in range(len(nums)):
        minind=i
        for j in range(i+1,len(nums)):
            if nums[minind]>nums[j]:
                minind=j
        nums[i],nums[minind]=nums[minind],nums[i]
    return nums
list_of_nums=eval(input())
result=selection_sort(list_of_nums)
print(result)# Selection sort and Insertion sort
```
ii)	#Insertion Sort
```
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: your name:Narendran.K
RegisterNumber: 23013500
def insertion_sort(nums):
    for i in range(1,len(nums)):
        key=nums[i]
        j=i-1
        while j>=0 and key<nums[j]:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=key
    return nums
list_of_nums = eval(input())
result=insertion_sort(list_of_nums)
print(result)
```

## Output:
##Selection sort:
![selection sort output](https://github.com/Narendran-sec/Sorting-Algorithm/assets/147473131/3a087e17-e688-4790-b377-eb94f137a976)
##insertion sort:
![Screenshot 2023-12-27 180526](https://github.com/Narendran-sec/Sorting-Algorithm/assets/147473131/bc9680eb-85af-4640-9568-123d9ac07f08)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
