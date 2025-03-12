def selection_sort(arr):
    n = len(arr)
    for i in range(n - 1):
        min_index = i  # Assume the first element is the smallest
        for j in range(i + 1, n):
            if arr[j] < arr[min_index]:
                min_index = j  # Update the index of the smallest element
        
        # Swap the found minimum element with the first element of the unsorted part
        arr[i], arr[min_index] = arr[min_index], arr[i]

# Example usage
arr = [64, 25, 12, 22, 11]
selection_sort(arr)
print("Sorted array:", arr)
