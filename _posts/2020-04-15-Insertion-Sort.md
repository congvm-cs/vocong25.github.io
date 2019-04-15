---
layout: post
title:  "Insertion Sort"
# date:   2018-9-23 23:45:13 +0700
subtitle: "In this project, I am going to implement INSERTION SORT"
author: vocong25
background: ''
tags: [algorithm, insertion_sort]
# comments: true
---


# Insertion Sort
---

## 1. Introduction

When we are working on an array of objects, we need to do some manipulations to reduce complexities or make problems much easier. To do that, some techniques have been applied. In this post, we mentions sorting of the array, **INSERTION SORT**.

## 2. Contents

### 2.1. Definition

**Input:** A sequence of n number $(a_1, a_2,..., a_n)$

**Output:** A permutation (reodering) $a'_1, a'_2,...,a'_n$ of the input sequence such that  $a'_1 \leq a'_2 \leq ... \leq a'_n$

### 2.2. Solution

![](/img/insertion_sort.jpg)

**Figure 2.1** The operation of Insertion sort on the array $A = (5, 2, 4, 6, 1, 3)$ 


**Explanation**

Updating ...

**Pseudo Code**

```math
**INSERTION-SORT(A)**
for j = 2 to A.length
    key = A[j]
    // Insert A[j] into the sorted sequence A[1 ... j-1]
    i = j - 1
    while i > 0 and A[i] > key
        A[i + 1] = A[i]
        i = i - 1
    A[i + 1] = key
```
### 2.3. Implementation

```C++
#include <iostream>
#include <vector>

std::vector<int> *InsertionSort(std::vector<int> (*arr))
{
    int n = (*arr).size();
    if (n < 1)
    {
        return arr;
    }
    else
    {
        for (int j = 1; j < n; j++)
        {
            int key = (*arr)[j];
            // Insert key into the sorted sequence (*arr)[0 .. j-1]
            int i = j - 1;
            while (i >= 0 & (*arr)[i] > key)
            {
                (*arr)[i + 1] = (*arr)[i];
                i = i - 1;
            }
            (*arr)[i + 1] = key;
        }
    }

    return arr;
}

int main(int argc, char const *argv[])
{
    std::vector<int> inputArr = {5, 2, 2, 6, 1, 2, 10};
    InsertionSort(&inputArr);
    return 0;
}
```
## Reference

1. **Latex symbols**: https://www.rpi.edu/dept/arc/training/latex/LaTeX_symbols.pdf
2. **Introduction of Algorithms**, 3rd, Cormen, Thomas H. and Leiserson, Charles E. and Rivest, Ronald L. and Stein, Clifford, The MIT Press
