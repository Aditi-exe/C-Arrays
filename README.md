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

### Code:

```
#include <stdio.h>

int main()
{
	int i, j;
	int x[5] = {2, 10, 15, 17, 21};
	
	
	// 3. storing and printing a string, which is essentially a character array, and then printing array elements at even indexes:
	
	char name[] = "SYMBIOSIS";
	printf("Value stored in the string (character array): %s \n\n", name);
	
	printf("String characters at even indexes: \n");
	
	for(j = 0; j < sizeof(name); j++)
	{
		if(j % 2 == 0)
		{
			printf("%c", name[j]);
		}
		else
		{
			printf("\n");
		}
	}
	
	
	
	
	
	// 2. taking an array index as input from the user and printing the element at that index in that array:
	
	//int user_index;
	
	//printf("Enter an array index: ");
	//scanf("%d", &user_index);
	
	//if((user_index < 0) || (user_index >= 4))
	//{
	//	  printf("invalid index \n\n");
	//}
	//else
	//{
	//    printf("Element at array index %d: %d \n\n", user_index, x[user_index]);
	//}
	
	
	
	
	// 1. printing the first array element along with the rest of the array using a for loop:
	
	//printf("First array element: %d \n\n", x[0]);
	
	//for(i = 0; i < 5; i++)
	//{
	//    printf("Array element %d: %d", i, x[i]);
	//	  printf("\n");
	//}
	
	
	return 0;
}
```

### Outputs:

![arrays.c output 1](https://github.com/Aditi-exe/C-Arrays/blob/main/L3_Arrays_1.PNG)

![arrays.c output 2](https://github.com/Aditi-exe/C-Arrays/blob/main/L3_Arrays_2.PNG)

![arrays.c output 3](https://github.com/Aditi-exe/C-Arrays/blob/main/L3_Arrays_3.PNG)

