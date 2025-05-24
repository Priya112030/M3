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
To write a C program to generate the Fibonacci series for the value 8.

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
 int n1=0,n2=1,n3,i,number=8;    

 
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
![image](https://github.com/user-attachments/assets/baabc72a-7ce0-48bb-b804-f952b14dbbf6)

## RESULT
Thus the program to generate the Fibonacci series for the value 8 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last second element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last second element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) scanf("%d", &arr[i]);
    if (n > 1) printf("%d\n", arr[n - 2]);
    else printf("Not enough elements\n");
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/29ff6563-b666-420a-ab19-73de0d8a8324)

## RESULT
Thus the program to read n elements as input and print the last second element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of negative elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be less 0 ,then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
 
 
int main()
{
    int a[100],i,n,c=0;
    scanf("%d", &n);
    for(i=0; i<n; i++)
    {
        scanf("%d", &a[i]);
    }
    for(i=0; i<n; i++)
    {
         
        if(a[i] < 0)
         c++;
    }
         printf("count  of negative numbers  in array: %d",c);
 
 
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/ef7abfb7-9594-4fa7-a309-04217ecc3394)

## RESULT
Thus the program to count total number of negative elements in an array has been executed successfully.


# EX -15 - Replace All Even Elements With '1' In One Dimensional Array
## Aim:
To write a C program to replace all odd elements with '1' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is odd (i.e., if the element modulo 2 equals 1).
3.	Replace even elements with '1':
     If an element is odd, replace that element with the character '1'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
# include <stdio.h>
int main()
{
    int arr[100],n,i;
    scanf("%d",&n);
    for(i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    for(i=0;i<n;i++){
        if(arr[i]%2!=0){
            arr[i]=1;
        }
    }
    for(i=0;i<n;i++){
        printf("%d ",arr[i]);
    }
    printf("\n");
    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/0b8287bd-fa08-4605-b01d-5077a8047b38)

## Result:
Thus, the program to replace all odd elements with '1' in one dimensional array was verified successfully.



