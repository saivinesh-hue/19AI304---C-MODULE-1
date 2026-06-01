# 19AI304 - Fundamentals of C Programming - Even Junior -2026

# IAPR 1 - Module 1

# Exp.1 : Display Character from ASCII Value

## Aim:

To write a C program that reads an integer value and displays its corresponding ASCII character.


## Algorithm:

1. Start the program.
2. Declare an integer variable num.
3. Read the integer input from the user using scanf().
4. Use the printf() function to display the corresponding ASCII character of the entered number using %c format specifier.
5. End the program.

## Program:

```c
#include <stdio.h>
int main()
{
    int num;
    scanf("%d", &num);
    printf("Character of ASCII Value %d is %c", num, num);
    return 0;
}
```

## Output:

<img width="780" height="199" alt="503051990-ed1ffff5-9456-476c-b00b-87bcc8810f8a" src="https://github.com/user-attachments/assets/f858f999-6c34-4205-afb2-533c902c1e94" />


## Result :

Thus, The program to write a C program that reads an integer value and displays its corresponding ASCII character was successfully executed.

***

# Exp.2 : Simple and Compound Interest Calculation

## Aim:

To write a C program that calculates both the Simple Interest (SI) and Compound Interest (CI) for a given principal, rate of interest, and time period.

## Algorithm:

1. Start the program.
2. Declare float variables principle, Year, rate, SI, and CI.
3. Read input values for principal, time (in years), and rate of interest using scanf().
4. Calculate Simple Interest using the formula:(Use pow() from math.h for exponentiation)
5. Print the calculated SI and CI using printf().
6. End the program.

## Program:

```c
#include <stdio.h>
#include <math.h>

int main()
{
 float principle, Year, rate, CI, SI;
 
 scanf("%f", &principle);
 scanf("%f", &Year);
 scanf("%f", &rate);
 
 SI = (principle * Year * rate) / 100;
 printf("Simple Interest = %.2f \n", SI);
 
 CI = principle * (pow((1 + rate / 100), Year));
 printf("Compound Interest = %.2f \n", CI);
 
 return 0;
}
```

## Output:

<img width="736" height="140" alt="503061099-8e45d22b-70b2-4fbb-af6a-c0ce5f74caa6" src="https://github.com/user-attachments/assets/a8988f96-c73d-42a3-bfef-c2c65ad472c8" />

## Result:

Thus, The C program that calculates both the Simple Interest (SI) and Compound Interest (CI) for a given principal, rate of interest, and time period was executed successfully.

***

# Exp.3 : Arithmetic Operations Using Switch Statement

## Aim:

To write a C program that performs basic arithmetic operations (+ and -) on two numbers using a switch statement.

## Algorithm:

1. Start the program.
2. Declare integer variables num1 and num2 for storing numbers, and a character variable op for the operator.
3. Read input values for num1, op, and num2 using scanf().
4. Use a switch statement to evaluate the operator:
5. Case '+' → Add num1 and num2 and print the result.
6. Case '-' → Subtract num2 from num1 and print the result.
7. Default → Print "Invalid Input" if the operator is not recognized.
8. End the program.

## Program:

```c
#include <stdio.h>
int main()
{
    int num1, num2;
    char op;
    scanf("%d %c %d", &num1, &op, &num2);
    
    switch (op) {
        case '+' :
            printf("Result = %d", num1 + num2);
            break;
        case '-' :
            printf("Result = %d", num1 - num2);
            break;
        default :
            printf("Invalid Input");
    }
    return 0;
}
```

## Output:

<img width="459" height="294" alt="503061965-36dc10bd-ebe5-47ae-970e-c0e5b78a1677" src="https://github.com/user-attachments/assets/61aa0bc5-228e-476c-9a0d-ccddbfb37c89" />

## Result:

Thus, The C program that performs basic arithmetic operations (+ and -) on two numbers using a switch statement was executed successfully.

***

# Exp.4 : Check if Number is Equal to 000

## Aim:

To write a C program that checks whether the input number is equal to 000.

## Algorithm:

1. Start the program.
2. Declare an integer variable num.
3. Read an integer input from the user using scanf().
4. Use an if statement to compare the number with 000.
5. If equal → print "Number is equal to 000".
6. Otherwise → print "Number is NOT equal to 000".
7. End the program.

## Program:

```c
#include <stdio.h>
int main()
{
    int num;
    scanf("%d", &num);
    if(num == 000)
        printf("Number is equal to 000");
    else
        printf("Number is NOT equal to 000");
    return 0;
}
```

# Output:

<img width="698" height="250" alt="503060066-5d7c460d-0b7b-4d8b-8d71-7134dd76bf13" src="https://github.com/user-attachments/assets/2883b6c2-dcbd-4593-959b-b38ee1803ca5" />

# Result:

Thus, The C program that checks whether the input number is equal to 000 was successfully executed.

***

# Exp.5 :  Grade Evaluation Based on Marks

## Aim:

To write a C program that reads a student's marks and prints the corresponding grade message.

## Algorithm:

1. Start the program.
2. Declare an integer variable marks.
3. Read the marks from the user using scanf().
4. Use if-else if-else statements to determine the grade:
5. Marks ≥ 70 → "VERY GOOD"
   + 60 ≤ Marks < 70 → "GOOD"
   +  50 ≤ Marks < 60 → "ABOVE AVERAGE"
   + 40 ≤ Marks < 50 → "AVERAGE"
6. Marks < 40 → "NEED TO IMPROVE"
7. Print the corresponding grade message.
8. End the program.

## Program:

```c
#include <stdio.h>
int main()
{
    int marks;
    scanf("%d", &marks);

    if (marks >= 70)
        printf("VERY GOOD");
    else if (marks >= 60)
        printf("GOOD");
    else if (marks >= 50)
        printf("ABOVE AVERAGE");
    else if (marks >= 40)
        printf("AVERAGE");
    else
        printf("NEED TO IMPROVE");

    return 0;
}
```

## Output:

<img width="475" height="291" alt="503062588-feb0daa9-8d10-43f7-a525-73cf950872b9" src="https://github.com/user-attachments/assets/05f3ed3f-02a1-4789-8dd6-73d130d35e6d" />

## Result:

Thus, The C program that reads a student's marks and prints the corresponding grade message was successfully executed.
