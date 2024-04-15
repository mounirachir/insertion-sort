# insertion-sort
Algorithm InsertionSort
    // Variable declaration and initialization
    length := 0
    comparisons := 0
    swaps := 0

    // Function definition
    For each element i in the range 1 to n-1, do
        key := arr[i]
        j := i - 1
        comparisons := comparisons + 1

        While j >= 0 and arr[j] > key, do
            arr[j + 1] := arr[j]
            j := j - 1
            swaps := swaps + 1
        End While

        arr[j + 1] := key
    End For

    // Return sorted array and metrics
    Return sortedArray := arr, comparisons := comparisons, swaps := swaps
End Algorithm
