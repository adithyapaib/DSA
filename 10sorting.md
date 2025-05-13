# Sorting Algorithms 
Sorting algorithms are a set of methods used to arrange elements in a specific order, typically in ascending or descending order. They are fundamental in computer science and are widely used in various applications, including data analysis, searching algorithms, and database management.

## 1. Bubble Sort  🫧

The bubble sort algorithm is a simple sorting algorithm that repeatedly steps through the list, compares adjacent elements and swaps them if they are in the wrong order. The crux of the algorithm is to put the largest unsorted element at the end of the list in each iteration.
### Algorithm
1. Start from the first element of the array.
2. Compare the current element with the next element.
3. If the current element is greater than the next element, swap them.
4. Move to the next element and repeat the process until the end of the array.
5. Repeat the process for the entire array until no swaps are needed, indicating that the array is sorted.

![Bubble Sort Animation](https://www.tutorialspoint.com/data_structures_algorithms/images/bubble_sort.gif)

> Sabse bada bulbula 🫧 End Mai Jayega

```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]
    return arr
```

### Time complexity
- Best case: O(n)
- Average case: O(n^2)
- Worst case: O(n^2)
### Space complexity
- O(1)
---

