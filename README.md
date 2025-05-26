

# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int num = 44;
    int shifts = 3;
    int result;

    result = num << shifts;

    printf("Original number: %d\n", num);
    printf("After left shifting by %d positions: %d\n", shifts, result);

    return 0;
}
```


## OUTPUT




![WhatsApp Image 2025-04-30 at 22 48 28_1c5ad919](https://github.com/user-attachments/assets/0fac2389-084a-4a29-bd57-f5a53674450a)





## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int num1, num2;

 
    printf("Enter first number: ");
    scanf("%d", &num1);

    printf("Enter second number: ");
    scanf("%d", &num2);

  
    if (num1 == num2) {
        printf("The two numbers are equal.\n");
    }

    
    if (num1 != num2) {
        printf("The two numbers are not equal.\n");
    }

    return 0;
}
```


## OUTPUT
![WhatsApp Image 2025-04-30 at 22 49 12_b70d6cdb](https://github.com/user-attachments/assets/3c0f8f11-d351-4764-b184-5c042f47e83d)


           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <ctype.h>

int main() {
    char str[100];
    int i = 0;


    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

   
    while (str[i]) {
        str[i] = tolower(str[i]);
        i++;
    }

    
    printf("Lowercase string: %s", str);

    
    return 0;
}
```

## OUTPUT
![WhatsApp Image 2025-04-30 at 22 49 45_37a5d61d](https://github.com/user-attachments/assets/335ea2d5-0fcf-4e41-91c0-041c3d33c4a0)




## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    char str[200];
    int i = 0, count = 1;

   
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

   
    do {
        if (str[i] == ' ' && str[i + 1] != ' ' && str[i + 1] != '\0') {
            count++;
        }
        i++;
    } while (str[i] != '\0');

    
    printf("Total number of words: %d\n", count);

   
    return 0;
}
```

## OUTPUT
![WhatsApp Image 2025-04-30 at 22 50 50_d8bee039](https://github.com/user-attachments/assets/cef0def7-3c66-446b-916c-63b72e63fcac)





## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    char c1[100], c2[100];
    int i = 0, flag = 0;

    
    printf("Enter first string: ");
    scanf("%[^\n]", c1);

  
    getchar();

   
    printf("Enter second string: ");
    scanf("%s", c2);

   
    do {
        if (c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    } while (c1[i] != '\0' || c2[i] != '\0');

   
    if (flag == 0)
        printf("Strings are same.\n");
    else
        printf("Strings are not same.\n");

   
    return 0;
}
```


## OUTPUT
 ![WhatsApp Image 2025-04-30 at 22 51 28_a14d4c7c](https://github.com/user-attachments/assets/3b692c6e-4de8-4920-b783-cd0485661754)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

