
# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int M, N;
    scanf("%d %d", &M, &N);
    int start = (M > N) ? M : N;
    int end = (M < N) ? M : N;
    if (start % 2 != 0) {
        start--;
    }
    for (int i = start; i >= end; i -= 2) {
        printf("%d ", i);
    }
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-04-27 143813](https://github.com/user-attachments/assets/4b894ff2-7a26-44f2-a5e9-cc4558bad0d9)

## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 

# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
## PROGRAM:
```
#include<stdio.h>
int main()
{
    int i,n,j;
    scanf("%d",&n);
    for(i=1;i<=n;i++)
    {
        for(j=1;j<=i;j++)
        {
            printf("%d ",j);
        }
        printf("\n");
    }
    return 0;
}

```

## OUTPUT:



![WhatsApp Image 2025-04-27 at 14 23 06_ecb915b9](https://github.com/user-attachments/assets/2b7f4fed-0828-4e18-b6bf-c76a79adc45f)

## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```

#include<stdio.h>
int add(int,int);
int sub(int,int);
int main()
{
    int a,b,c,d;
    scanf("%d%d",&a,&b);
    c = add(a,b);
    d = sub(a,b);
    printf("Addition: %d\n",c);
    printf("Subtraction: %d",d);
}
int add(int x,int y)
{
    int z;
    z = x + y;
    return z;
}
int sub(int x,int y)
{
    int z;
    z = x - y;
    return z;
}

```


## OUTPUT:
![Screenshot 2025-04-27 144029](https://github.com/user-attachments/assets/8a18dfbe-70ed-460a-86ae-71ceedd81540)



## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int a,b,sum=0,i;
    scanf("%d%d",&a,&b);
    for(i=a;i<=b;i++)
    {
        if(i%2!=0)
        {
            sum += i;
        }
    }
    printf("%d",sum);
    return 0;
}

```

## OUTPUT:

![Screenshot 2025-04-27 144125](https://github.com/user-attachments/assets/b5370853-a818-4d13-a176-a34063fc3e08)


## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int n,fact=1;
    scanf("%d",&n);
    for(int i=1;i<=n;i++)
    {
        fact*=i;
    }
    printf("Factorial value is: %d",fact);
    return 0;
}

```



## OUTPUT:
![Screenshot 2025-04-27 144231](https://github.com/user-attachments/assets/35994c76-704c-47a9-b5df-41b0150fa6e9)




## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
