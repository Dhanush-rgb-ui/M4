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
```c
#include <stdio.h>

int main() {
    int a = 44; 
    int b = 3;  
    int result;

    
    result = a << b;

    
    printf("Original number: %d\n", a);
    printf("After left shifting %d by %d positions: %d\n", a, b, result);

    return
}
```


## OUTPUT

<img width="1631" height="530" alt="image" src="https://github.com/user-attachments/assets/817a0e30-ad85-4c93-ad10-abd0d59c3ed0" />








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
```c
#include <stdio.h>

int main() {
    int num1, num2;

    printf("Enter the first number: ");
    scanf("%d", &num1);

    printf("Enter the second number: ");
    scanf("%d", &num2);

    if(num1 == num2) {
        printf("Both numbers are equal.\n");
    } else {
        printf("Both numbers are not equal.\n");
    }

    return 0;
}

```


## OUTPUT
<img width="1627" height="582" alt="image" src="https://github.com/user-attachments/assets/29686c83-cfe8-4af7-9eed-54af2f8bf909" />

           
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
```c
#include <stdio.h>
#include <ctype.h>  // For tolower() function

int main() {
    char str[100];
    int i = 0;

    // Read a string from the user
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);  // Reads string with spaces

    // Convert each character to lowercase
    while(str[i] != '\0') {
        str[i] = tolower(str[i]);
        i++;
    }

    // Display the result
    printf("Lowercase string: %s\n", str);

    return 0;
}
```

## OUTPUT
<img width="1623" height="611" alt="image" src="https://github.com/user-attachments/assets/682bd87c-7545-483d-bba9-937050ed9cb6" />





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
```c
#include<stdio.h>
int main(){
    char a[100];
    printf("Enter a string: ");
    scanf("%[^\n]",a);
    int i,count=0;
    for(i=0;a[i]!='\0';i++){
        if(a[i-1]==' ' || a[i+1]=='\0'){
            count+=1;
        }
    }
    printf("\nNo of Words: %d",count);
    return 0;
}


```

## OUTPUT

<img width="1633" height="480" alt="image" src="https://github.com/user-attachments/assets/4d24fc45-53c6-48bf-af97-87ecf5f2d667" />




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
```c
#include <stdio.h>

int main() {
    char c1[100], c2[100];
    int i = 0, flag = 0;

    // Read first string (can include spaces)
    printf("Enter the first string: ");
    scanf(" %[^\n]", c1);  // Space before % to ignore any leftover newline

    // Read second string (no spaces)
    printf("Enter the second string: ");
    scanf("%s", c2);

    // Compare characters one by one
    while(c1[i] != '\0' && c2[i] != '\0') {
        if(c1[i] != c2[i]) {
            flag = 1;  // Strings differ
            break;
        }
        i++;
    }

    // If one string is longer than the other
    if(c1[i] != '\0' || c2[i] != '\0') {
        flag = 1;
    }

    // Display result
    if(flag == 0) {
        printf("Strings are same.\n");
    } else {
        printf("Strings are not same.\n");
    }

    return 0;
}
```


## OUTPUT
 <img width="1631" height="835" alt="image" src="https://github.com/user-attachments/assets/42f7d0a1-5897-4f94-98c6-6ee9b634eb77" />


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

