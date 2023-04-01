# **Arrays in C**

In C, an array is a collection of elements of the same data type, which are stored in a contiguous block of memory. 
Each element of an array can be accessed by its index, which is an integer value that represents the position of the element in the array.

An array can be represented as follows:

![A representation of a one-dimensional array in C](https://cdn.programiz.com/sites/tutorial2program/files/c-arrays.jpg)

Array indexing starts from 0 and not 1. 

Consider the following example:

```
int arr[5] = {2, 7, 4, 9, 0};
```

The array arr is an integer array that consists of 5 elements. The elements are indexed from 0 through 4, so to retrieve the 3rd element of arr, the following code will have to be used:

```
printf("%d", arr[2]);
```

This will display 4 as the output, since it is the third element in the array but is indexed 2.

Arrays can have integer, float, character or string elements among other data types. The data type must be specified while declaring the array.
Arrays can be dynamically filled by taking user input in the body of a for loop being executed the same number of times as the size of the array.

Other array declarations include:

```
char ch_arr[3] = {'a', 'b', 'c'};
float f_arr[4] = {100.3, 45.97, 26.11, 9.8};
```

The program in this repository puts forth some uses of arrays and operations that can be performed on them.

