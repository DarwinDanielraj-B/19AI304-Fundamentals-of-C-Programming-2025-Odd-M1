# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
~~~
#include <stdio.h>
int main()
{
    printf("Integer Literal = %d\n", 10);
    printf("Size of Integer = %lu bytes\n", sizeof(10));

    printf("Float Literal = %.2f\n", 3.14);
    printf("Size of Float = %lu bytes\n", sizeof(3.14f));

    printf("Character Literal = %c\n", 'A');
    printf("Size of Character = %lu bytes\n", sizeof('A'));

    printf("String Literal = %s\n", "Hello C");
    printf("Size of String = %lu bytes\n", sizeof("Hello C"));

    return 0;
}
~~~
# Output:
<img width="451" height="397" alt="Screenshot 2026-05-31 075605" src="https://github.com/user-attachments/assets/03e6fb61-ca70-4c48-a855-e2ec30b1c171" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
~~~
#include <stdio.h>

#define PI 3.14159

int main()
{
    const int DAYS = 7;

    printf("Value of PI = %.5f\n", PI);
    printf("Value of DAYS = %d\n", DAYS);

    return 0;
}
~~~
# Output:
<img width="396" height="214" alt="Screenshot 2026-05-31 080806" src="https://github.com/user-attachments/assets/d0a078d7-d66e-4305-97ff-69a81ebc83c0" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
~~~
#include <stdio.h>

int main()
{
    int num;
    float f;
    double d;
    char ch;
    scanf("%d", &num);
    scanf("%f", &f);
    scanf("%lf", &d);
    scanf(" %c", &ch);

    printf("\nInteger = %d\n", num);
    printf("Float = %f\n", f);
    printf("Double = %lf\n", d);
    printf("Character = %c\n", ch);

    return 0;
}
~~~
# Output:
<img width="386" height="499" alt="Screenshot 2026-05-31 080715" src="https://github.com/user-attachments/assets/dfb2dace-2c9a-4792-b59f-14f9cabeb3b4" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
~~~
#include <stdio.h>

int main()
{
    int a, b;
    scanf("%d %d", &a, &b);

    printf("\nArithmetic Operations\n");
    printf("Addition = %d\n", a + b);
    printf("Subtraction = %d\n", a - b);
    printf("Multiplication = %d\n", a * b);
    printf("Division = %d\n", a / b);
    printf("Remainder = %d\n", a % b);

    printf("\nBitwise Operations\n");
    printf("AND = %d\n", a & b);
    printf("OR = %d\n", a | b);
    printf("XOR = %d\n", a ^ b);
    printf("Left Shift = %d\n", a << b);
    printf("Right Shift = %d\n", a >> b);
    printf("NOT of a = %d\n", ~a);
    printf("NOT of b = %d\n", ~b);

    return 0;
}
~~~
# Output:
<img width="463" height="640" alt="Screenshot 2026-05-31 080456" src="https://github.com/user-attachments/assets/953101d7-167c-4e05-8391-23ca9b438094" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
~~~
#include <stdio.h>

int main()
{
    char ch;
    scanf("%c", &ch);

    (ch >= '0' && ch <= '9') ? printf("Digit") :
    ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) ?
    ((ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||
      ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') ?
      printf("Vowel") : printf("Consonant"))
    : printf("Special Symbol");

    return 0;
}
~~~
# Output:
<img width="409" height="234" alt="Screenshot 2026-05-31 080239" src="https://github.com/user-attachments/assets/0860b335-0868-4554-97cf-fcf0f98ce94a" />
<img width="418" height="238" alt="Screenshot 2026-05-31 080214" src="https://github.com/user-attachments/assets/6094c339-a9b6-4bdf-b6c9-2b45bae7c612" />
<img width="387" height="246" alt="Screenshot 2026-05-31 080156" src="https://github.com/user-attachments/assets/0d38bbbc-b5d2-452c-b694-fca70b407b2d" />
<img width="395" height="207" alt="Screenshot 2026-05-31 081138" src="https://github.com/user-attachments/assets/36dc7e2a-a52d-4286-98ed-da7dd90d7d36" />


# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


