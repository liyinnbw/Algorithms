# Algorithms
- [Random](#random)
- [Binary Search](#binary-search)

## Dynamic Programming


## Random
<details>
<summary>Reservoir Sampling</summary>

[Reservoir Sampling](https://en.wikipedia.org/wiki/Reservoir_sampling)

Draw k items without replacement from N items with equal probability. Good for unknown N.

Algorithm Sketch:
1. Init an array of size k. Process the incoming items as the following:
2. First k items are straight away put inside the bin
3. For each of subsequent n-th item, generate a random number x in [1,n]. If x in [1,k], replace x-th item in the bin with this new item.

</details>

## Binary Search
<details>
<summary>Order Static Tree</summary>

[Order Static Tree](https://en.wikipedia.org/wiki/Order_statistic_tree)

Standard BST plus size of subtree info at every node. 
In addition to BST properties, OST also provides:
1. O(logN) search time for k-th item (if the tree is balanced)
2. O(1) time to tell the index of a given node (size-right.size-1)

Sample Problems:
- [Find k-th item](https://www.hackerearth.com/practice/algorithms/searching/binary-search/practice-problems/algorithm/victory-over-power-4a0cb459/)

</details>

<details>
<summary>Binary Indexed Tree</summary>

[Binary Indexed Tree](https://cs.stackexchange.com/questions/10538/bit-what-is-the-intuition-behind-a-binary-indexed-tree-and-how-was-it-thought-a)

Good for:
1. O(logN) time to tell the accumulated sum of array values at any index (array size must be fixed)
2. O(logNlogN) search time for k-th item (if there are limited number of possible items)

Sample Problems:
- [Range sum](https://leetcode.com/problems/range-sum-query-mutable/)
- [Find k-th item](https://www.hackerearth.com/practice/algorithms/searching/binary-search/practice-problems/algorithm/victory-over-power-4a0cb459/) (creative use)


</details>
