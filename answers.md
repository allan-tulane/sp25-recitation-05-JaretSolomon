# CMPS 2200 Reciation 5
## Answers

**Name:** Jaret Solomon


Place all written answers from `recitation-05.md` here for easier grading.


Compare running times using `compare-sort` between variants of
Quicksort and the
provided implementation of selection sort (`ssort`). Perform two
different comparisons: a comparison between sorting methods using
random permutations of the specified sizes, and a comparison using
already sorted permutations. How do the running times compare to the
asymptotic bounds? How does changing the type of input list change the
relative performance of these algorithms? Note that you may have to
modify the list sizes based on your system memory; compare at least 10
different list sizes. The `print_results` function in `main.py` gives
a table of results, but feel free to use code from Lab 1 to plot
the results as well. 




- **1b.**
|      n |   qsort-fixed-pivot |   qsort-random-pivot |   time-sort||time-sort |
|--------|---------------------|----------------------|------------||----------|
|    100 |               0.097 |                0.118 |      0.010 |
|    200 |               0.187 |                0.226 |      0.018 |
|    500 |               0.578 |                0.733 |      0.053 |
|   1000 |               1.226 |                1.314 |      0.115 |Recursion Depth (< 1000)
|   2000 |               2.657 |                3.006 |      0.244 |
|   5000 |               6.806 |                7.816 |      0.659 |
|  10000 |              14.685 |               17.689 |      1.423 |
|  20000 |              31.648 |               36.761 |      3.076 |
|  50000 |              86.366 |              101.339 |      8.638 |
| 100000 |             178.054 |              198.197 |     18.293 |


Quicksort average case: O(n log n) Quicksort worst case: O(n^2) Selection sort average case: O(n^2) Selection sort worst case: O(n^2)


- **1c.**


Python uses a sorting algorithm called [*Timsort*](https://en.wikipedia.org/wiki/Timsort), designed by Tim Peters. Compare the fastest of your sorting implementations to the Python
sorting function `sorted`, conducting the tests in 1b above. 

1c. tim-sort can be seen in the table above. It is faster than any of the other algorithms implemented in this lab.
