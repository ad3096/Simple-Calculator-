# Simple-Calculator-
This is simple calculator made by C language which can do addition,Substraction ,multiplication and division 

#include <stdio.h>

int factorial(int n) {
    if (n == 0 || n == 1) {
        return 1; 
    } 
    else {
        return n * factorial(n - 1); 
    }
}

int main() {
    int num;

    printf("Enter a number to calculate its factorial: ");
    scanf("%d", &num);

    if (num < 0) {
        printf("factorial error\n");
    } 
    else {
        printf("The factorial of %d is = %d\n",
         num, factorial(num));
    }

    return 0;
}
