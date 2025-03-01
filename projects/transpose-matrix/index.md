---
title: Transpose Matrix in Every Language
layout: default
date: 2020-10-08
last-modified: 2021-10-06
featured-image:
tags: [transpose-matrix]
authors: 
  - DedAvocado
---

In this article, we'll demonstrate how to find Transpose of a Matrix, its requirements, and how
to test it.

## Description

In linear algebra, the transpose of a matrix is an operator which flips a matrix over its diagonal; 
that is, it switches the row and column indices of the matrix A by producing another matrix, often 
denoted by Aᵀ. For example, the following matrix could be the matrix A:

| 1 | 2 | 3 |
| - |:-:| -:|
| 4 | 5 | 6 |
| 7 | 8 | 9 |

Once transposed, A becomes the following matrix, Aᵀ:

| 1 | 4 | 7 |
| - |:-:| -:|
| 2 | 5 | 8 |
| 3 | 6 | 9 |

The transpose of a matrix was introduced in 1858 by the British mathematician Arthur Cayley.

## Requirements

For the purposes of this project, we'll ask that you create a program which accepts
a matrix as a list of integers and the dimensions of that matrix in the following
format:

```
transpose-matrix.lang 3 3 "1, 2, 3, 4, 5, 6, 7, 8, 9"
```

Here, the first two input numbers indicate the column and row size of the matrix, respectively, and the 
next input is the list of numbers to be included in the matrix.

## Testing

Verify that the actual output matches the expected output (see [requirements][1])

| Description             | Cols  | Rows  | Matrix                 | Output                                                                    |
| ----------------------- |:-----:|:-----:|:----------------------:| -------------------------------------------------------------------------:|
| No input                |       |       |                        | Usage: please enter the dimension of the matrix and the serialized matrix |
| Missing input: Size     |       |       | ```1, 2, 3, 4, 5, 6``` | Usage: please enter the dimension of the matrix and the serialized matrix |
| Missing input: integers | 3     | 3     |                        | Usage: please enter the dimension of the matrix and the serialized matrix |
| Sample input            | 3     | 2     | ```1, 2, 3, 4, 5, 6``` | ```1, 4, 2, 5, 3, 6```                                                    |

## Articles

{% include article_list.md collection=site.categories.transpose-matrix %}
