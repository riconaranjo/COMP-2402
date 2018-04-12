# Summary Tables

These are all the tables summarizing the comparisons between different data structures and algorithms covered in this course.

## Access and Modifification Characteristics

|            | get/set             | add/remove          |
|------------|---------------------|---------------------|
| Arrays     | _O(1)_              | _O(1 + min(i,n-i))_ |
| LinkedList | _O(1 + min(i,n-i))_ | _O(1)`*`_           |
| Skiplist   | _O(log n)_          | _O(log n)_          |

`*given a pointer to the location, else traversal is necessary`

## Binary Search Tree Implementations

|                       | find()                 | add()                  | remove()               |
|------------------|------------------------|------------------------|------------------------|
| BST                   | _O(n)_                 | _O(n)_                 | _O(n)_                 |
| RBST / Treaps         | _O(log n)_ [expected]  | _O(log n)_ [expected]  | _O(log n)_ [expected]  |
| Scapegoat Trees       | _O(log n)_ [amortized] | _O(log n)_ [amortized] | _O(log n)_ [amortized] |
| 2-4 / RedBlack Trees  | _O(log n)_ [worst-case] | _O(log n)_ [worst-case] | _O(log n)_ [worst-case] |

## Sorted Set Implementations

|                          | Runtime                 |
|--------------------------|-------------------------|
| Skiplists                | _O(log n)_ [expected]   |
| Treaps                   | _O(log n)_ [expected]   |
| Scapegoat Trees          | _O(log n)_ [amortized]  |
| **2-4 / RedBlack Trees** | _O(log n)_ [worst-case] |

## Comparison-based Algorithms

|            | Comparisons                      | In-place | Stable |
|------------|----------------------------------|----------|--------|
| Merge Sort | _n•log(n)_ [worst-case]          | no       | yes    |
| Heap Sort  | _1.38n•log(n) + O(n)_ [expected] | yes      | no     |
| Quick Sort | _2n•log(n) + O(n)_ [worst-case]  | yes      | no     |