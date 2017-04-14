Highly efficient implementation of [introsort](https://en.wikipedia.org/wiki/Introsort) (introspective sort) algorithm, hybrid of quicksort, heapsort, and insertion sort that has particularly good runtime behavior.  It is one of the fastest comparison sorting, algorithms in use today, and is the usual implementation of the std::sort algorithm provided with the C++ STL.

Key attributes of this implementation:
* 3-way partition 
* median of three (using 3 randomly chosen elements) for pivot selection
* sorting networks for 1 &le; N &le; 6
* insertion sort for 7 &le; N &le; 25
* Quicksort uses only one recursive call (the other one is transformed into tail recursion)
* std::heap_sort if Quicksort degenerates


Test cases used in testing and benchmarking:
 *  0 -> N = 100;          V = 100
 *  1 -> N = 1'000;        V = 500
 *  2 -> N = 10'000;       V = 2'000
 *  3 -> N = 100'000;      V = 15'000
 *  4 -> N = 1'000'000;    V = 40'000
 *  5 -> N = 5'000'000;    V = 80'000
 *  6 -> N = 10'000'000;   V = 125'000
 *  7 -> N = 100;          V = 2'000'000'000
 *  8 -> N = 1'000;        V = 2'000'000'000
 *  9 -> N = 10'000;       V = 2'000'000'000
 * 10 -> N = 100'000;      V = 2'000'000'000
 * 11 -> N = 1'000'000;    V = 2'000'000'000
 * 12 -> N = 5'000'000;   V = 2'000'000'000
 * 13 -> N = 10'000'000;  V = 2'000'000'000

![](https://github.com/AlexandruValeanu/Algorithms-and-Data-Structures/blob/master/Introsort/charts/figure_0.png)
![](https://github.com/AlexandruValeanu/Algorithms-and-Data-Structures/blob/master/Introsort/charts/figure_1.png)
![](https://github.com/AlexandruValeanu/Algorithms-and-Data-Structures/blob/master/Introsort/charts/figure_2.png)
![](https://github.com/AlexandruValeanu/Algorithms-and-Data-Structures/blob/master/Introsort/charts/figure_3.png)
![](https://github.com/AlexandruValeanu/Algorithms-and-Data-Structures/blob/master/Introsort/charts/figure_4.png)
![](https://github.com/AlexandruValeanu/Algorithms-and-Data-Structures/blob/master/Introsort/charts/figure_5.png)
![](https://github.com/AlexandruValeanu/Algorithms-and-Data-Structures/blob/master/Introsort/charts/figure_6.png)