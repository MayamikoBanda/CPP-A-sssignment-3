# CPP-A-sssignment-3
OBJECT ORIENTED PROGRAMMING ASSIGNMENT 3 

 

QUESTION 1 

#include <stdio.h> 

int main(void) {int i, j; const int ROW = 3; const int COL = 4; 

int arr[ROW][COL] = { 
   {1, 2, 3, 4}, 
   {5, 6, 7, 8}, 
   {9, 10, 11, 12} 
}; 
 
printf(">>> *( *(arr+i)+j ) <<<\n"); 
for(i = 0; i < ROW; i++) { 
   for(j = 0; j < COL; j++) { 
       printf("%4d", *(*(arr+i) + j)); 
   } 
   printf("\n"); 
} 
 
printf("\n"); 
 
printf(">>> arr[i][j] <<<\n"); 
for(i = 0; i < ROW; i++) { 
   for(j = 0; j < COL; j++) { 
       printf("%4d", arr[i][j]); 
   } 
   printf("\n"); 
} 
 
printf("\n"); 
 
return 0; 
 

} 

CODE EXPLAINATION  

This program works with a 2D array (arr[3][4]) and prints its values in two different ways: 

1. Using pointer notation 

FUNCTION: ((arr+i) + j) 

arr is treated as a pointer to rows  

arr + i → moves to the i-th row  

*(arr + i) → gives the row  

+ j → moves to the j-th column  

Final * → gets the actual value 

So this accesses the same element as arr[i][j], but using pointers. 

2. Using array notation 

arr[i][j] 

Direct and easier way to access elements  

i = row index  

j = column index 

In conclusion; Both methods access the same memory locations, just written differently. 

Hence:  arr[i][j] ≡ ((arr+i) + j) 

 

 
