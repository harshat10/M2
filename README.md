## NAME: HARSHAT.G
## REG NO.: 212224040106
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
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    for (int i=1;i<a;i++){
        printf("%d, ",i);
    }
    printf("%d",a);
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-05-11 194026](https://github.com/user-attachments/assets/ff88ee49-01af-497a-8b5e-2c18e8eb695a)

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
```
#include <stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    for (int i=a;i>0;i--){
        for (int j=0;j<i;j++){
            printf("*");
        }
        printf("\n");}
}
```
## OUTPUT:
![Screenshot 2025-05-11 194217](https://github.com/user-attachments/assets/db912601-30ab-4438-b35f-79f78455d627)

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
#include <stdio.h>
int add();
int subtract();

int main() {
    int sum, difference;

    sum = add();          
    printf("Addition: %d\n", sum);

    difference = subtract();  
    printf("Subtraction: %d\n", difference);

    return 0;
}
int add() {
    int num1, num2;
    scanf("%d %d", &num1, &num2);
    return num1 + num2;
}
int subtract() {
    int num1, num2;
    scanf("%d %d", &num1, &num2);
    return num1 - num2;
}

```
## OUTPUT:
![Screenshot 2025-05-11 194318](https://github.com/user-attachments/assets/e0e8458c-729a-4e30-a2c6-fa51de792f13)

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
int main(){
    int a,result = 0,q,reminder;
    scanf("%d",&a);
    q=a;
    while(q!=0){
        reminder = q%10;
        result = result*10+reminder;
        q = q/10;
    }
    if (result == a){
        printf("Palindrome Number");
    }
    else{
        printf("Not a Palindrome Number");
    }return 0;
}
```
## OUTPUT:
![Screenshot 2025-05-11 194414](https://github.com/user-attachments/assets/b7c1f82a-9a60-477e-b566-6b3513ca0238)

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
## OUTPUT:
![437939385-35994c76-704c-47a9-b5df-41b0150fa6e9](https://github.com/user-attachments/assets/6a4be79a-64b0-4e64-9d1c-054efdbba40e)
## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
