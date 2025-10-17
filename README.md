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
    int a = 44;
    int b = 3;
    int result;

    result = a << b;

    printf("The result of left shifting %d by %d positions is: %d\n", a, b, result);

    return 0;
}
```
## OUTPUT

<img width="587" height="121" alt="image" src="https://github.com/user-attachments/assets/fb846f9f-3661-4b86-b3e4-a7f398a87a19" />








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

    if (num1 == num2)
        printf("Both numbers are equal.\n");

    if (num1 != num2)
        printf("Both numbers are not equal.\n");

    return 0;
}
```

## OUTPUT
<img width="280" height="165" alt="image" src="https://github.com/user-attachments/assets/8977cd99-76d1-4b8a-a2d8-2201b5ab5136" />
<img width="300" height="157" alt="image" src="https://github.com/user-attachments/assets/fffe4a21-f2dd-4f21-96f0-82b01c54b0ee" />
     
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
    int i;

    printf("Enter a string: ");
    scanf("%s", str);

    for (i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }

    printf("String in lowercase: %s\n", str);

    return 0;
}
```
## OUTPUT
<img width="348" height="129" alt="image" src="https://github.com/user-attachments/assets/a768997d-54bc-43dc-960d-9a09239e1c50" />




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
    scanf(" %[^\n]", str); // reads string with spaces

    do {
        if (str[i] == ' ' || str[i] == '\t')
            count++;
        i++;
    } while (str[i] != '\0');

    printf("Total number of words in the string: %d\n", count);

    return 0;
}
```
## OUTPUT
<img width="492" height="133" alt="image" src="https://github.com/user-attachments/assets/b65641b6-c855-4f9a-9b9a-286d9c5b457f" />





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

    printf("Enter second string: ");
    scanf(" %s", c2);

    while (c1[i] != '\0' && c2[i] != '\0') {
        if (c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    }

    if (c1[i] != '\0' || c2[i] != '\0')
        flag = 1;

    if (flag == 0)
        printf("Strings are same.\n");
    else
        printf("Strings are not same.\n");

    return 0;
}
```

## OUTPUT
<img width="374" height="170" alt="image" src="https://github.com/user-attachments/assets/d9888c15-e8d9-41ba-862f-46c2e9b930ce" />
<img width="350" height="157" alt="image" src="https://github.com/user-attachments/assets/2cd8a2e8-0d49-445b-b3fc-0b6551e1d744" />



## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

