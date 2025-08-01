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
    int result = a << b;
    printf("Result after left shifting %d by %d times is: %d\n", a, b, result);
    return 0;
}
```
## OUTPUT
<img width="657" height="85" alt="438794272-0cfe2107-ce78-4ded-a55f-78182fc59ddc" src="https://github.com/user-attachments/assets/802f0e33-2048-46bf-9f45-9764b224c771" />









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
    
    if(num1 == num2) {
        printf("Both are equal\n");
    } else {
        printf("Both are not equal\n");
    }

    return 0;
}
```


## OUTPUT
<img width="517" height="139" alt="438794466-751b01c8-7a44-48e8-ada2-9b38f8462640" src="https://github.com/user-attachments/assets/2492d385-b7ee-463e-b87b-baa841198a73" />

           
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
    
    printf("Enter a string: ");
    scanf("%s", str);
    
    for(int i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }
    
    printf("Lowercase string: %s\n", str);
    
    return 0;
}
```

## OUTPUT
<img width="570" height="111" alt="438794691-1f550805-248c-4e13-84de-f6683c21dac8" src="https://github.com/user-attachments/assets/2411995b-1dc4-48ff-bc8c-c6ccf0bbe4f7" />




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
    char str[100];
    int count = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    for(int i = 0; str[i] != '\0'; i++) {
        if(str[i] == ' ') {
            count++;
        }
    }

    printf("Number of spaces: %d\n", count);
    
    return 0;
}

```

## OUTPUT
<img width="585" height="115" alt="438794835-0e11a354-d45f-4263-8c47-8227bd5fc687" src="https://github.com/user-attachments/assets/5f8fda35-5a2f-4ceb-87a9-8fb4a6c62552" />





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
    int flag = 0, i = 0;

    
    printf("Enter the first string: ");
    scanf("%[^\n]", c1);

    
    getchar();  
    printf("Enter the second string: ");
    scanf("%s", c2);

    
    while(c1[i] != '\0' && c2[i] != '\0') {
        
        if(c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    }

    if(flag == 0 && c1[i] == c2[i]) {
        printf("Strings are same\n");
    } else {
        printf("Strings are not same\n");
    }

    return 0;
}
```


## OUTPUT
 <img width="550" height="136" alt="438795038-327b122e-1d43-4e9a-92c5-521fddfce703" src="https://github.com/user-attachments/assets/f695e4ad-556a-4aab-86b3-e7875106ace5" />


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

