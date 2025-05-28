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

int main()
{
    int number = 44;
    int shifts = 3;
    int result = number << shifts;  
    printf("Original number: %d\n", number);
    printf("After left shifting by %d bits: %d\n", shifts, result);

    return 0;
}
```

## OUTPUT

![Screenshot 2025-05-28 101120](https://github.com/user-attachments/assets/c88292b7-d945-4adb-ac4c-9db646056d3c)










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

int main()
{
    int num1, num2;
    scanf("%d", &num1);
    scanf("%d", &num2);
    if (num1 == num2) {
        printf("The numbers are equal.\n");
    }

    return 0;
}
```

## OUTPUT


![Screenshot 2025-05-28 101404](https://github.com/user-attachments/assets/b26dcfd0-2507-43cf-a73b-bb82da15cdf3)


           
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

int main()
{
    char str[100];
    fgets(str, sizeof(str), stdin);  
    for (int i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }

    printf("Lowercase string: %s\n", str);

    return 0;
}
```

## OUTPUT

![Screenshot 2025-05-28 101624](https://github.com/user-attachments/assets/397d08cf-2fd3-430e-8cf6-ca8f0d2e0b17)



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
#include <ctype.h>

int main()
{
    char str[200];
    int i = 0, wordCount = 0;
    int inWord = 0;  
    fgets(str, sizeof(str), stdin);
    do {
        char ch = str[i];
        if (ch != ' ' && ch != '\n' && ch != '\t' && ch != '\0') {
            if (!inWord) {
                wordCount++;  
                inWord = 1;
            }
        } else {
            inWord = 0;  
        }
        i++;
    } while (str[i] != '\0');

    printf("Total number of words: %d\n", wordCount);

    return 0;
}
```
## OUTPUT


![Screenshot 2025-05-28 102001](https://github.com/user-attachments/assets/99ac71d6-d0e2-4d26-b642-d46fcd8d0f56)



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
#include<stdio.h>
int main()
{
    char str1[100], str2[100];
    int i,f=0;
    scanf("%s", str1);
    scanf("%s", str2);
    for (i=0; str1[i] != '\0'; i++){
        if (str1[i] != str2[i]){
            f=1;
            break;
        }
    }
    if (f == 1){
        printf("strings are not same\n");
    } else {
        printf("strings are same\n");
    }
    return 0;
}
```

## OUTPUT
 ![Screenshot 2025-05-28 102342](https://github.com/user-attachments/assets/09b105f6-7042-486d-aaa8-d6bed038f115)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

