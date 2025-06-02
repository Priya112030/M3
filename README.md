# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>
void emi_calculator(float principal, float rate, int time);

int main() {
    float principal, rate;
    int time;
    scanf("%f", &principal);
    scanf("%f", &rate);
    scanf("%d", &time);
    emi_calculator(principal, rate, time);
    return 0;
}

void emi_calculator(float principal, float rate, int time) {
    float monthly_rate = rate / (12 * 100);
    int months = time * 12;
    float emi;

    emi = (principal * monthly_rate * pow(1 + monthly_rate, months)) /
          (pow(1 + monthly_rate, months) - 1);

    printf("Monthly EMI is= %.3f\n", emi);
}

```

## OUTPUT
![image](https://github.com/user-attachments/assets/24bfbc3b-0627-4102-9e35-d59d5beee7ec)

## RESULT
Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 
## EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include<stdio.h>    
int main()    
{    
 int n1=0,n2=1,n3,i,number;    
 scanf("%d",&number);
 
 printf("%d %d",n1,n2);
i=2;
 while(i<number)
 {    
  n3=n1+n2;    
  printf(" %d",n3);    
  n1=n2;    
  n2=n3; 
  i++;
 }  
  return 0;  
 }
```

## OUTPUT
![Screenshot 2025-04-27 150452](https://github.com/user-attachments/assets/cdc27f77-0a25-4bf3-8a0e-7ef322435607)


## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last  element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last  element.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int arr[n];
    for (i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    if (n>0) printf("%d\n",arr[n-1]);
    else printf(" ");   
}
```

## OUTPUT
![Screenshot 2025-04-27 150543](https://github.com/user-attachments/assets/34851039-ad90-4502-b85c-dc0c5777a8a6)


## RESULT
Thus the program to read n elements as input and print the last  element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, i, count = 0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements: %d\n", count);

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/19b4585f-7b93-4f89-b648-92be797fcd68)



## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array
## Aim:
To write a C program to replace all odd elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);

    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';  // Replacing even numbers with 'E'
        }
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    return 0;
}
```

## Output:
![WhatsApp Image 2025-04-27 at 15 09 19_29145594](https://github.com/user-attachments/assets/8069572d-0579-4e34-acf8-50030e3aea5f)

## Result:
Thus, the program to replace all odd elements with 'E' in one dimensional array was verified successfully.



