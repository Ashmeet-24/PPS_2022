## Program 38 : Write a program using Recursion.
```C
#include<stdio.h>
long int fact(int n);
int main() 
{
    int n;
    printf("Enter a positive integer: ");
    scanf("%d",&n);
    printf("Factorial of %d = %ld", n, fact(n));
    return 0;
}
long int fact(int n) 
{
    if (n>=1)
        return n*fact(n-1);
    else
        return 1;
}
```
**Output :**
```C
Enter a positive integer: 31
Factorial of 31 = 738197504
