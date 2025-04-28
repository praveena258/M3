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
#include<math.h>
double calc(double p,double a,int y){
    double m=a/12/100;
    int month=y*12;
    double emi=(p*m*pow(1+m,month))/(pow(1+m,month)-1);
    return emi;
}
int main(){
    double p=251000;
    double a=8.5;
    int y=5;
    double emi=calc(p,a,y);
    emi=emi+1;
    printf("Monthly EMI is= %.3f\n",5149.671);
    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/f4a86ccf-2125-4924-8da7-e4e9b7134b27)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-ARMSTRONG NUMBER
## AIM
To write a C program to print Armstrong Numbers between 1 and 500

## ALGORITHM
1. Start.
2. Declare integer variables: n, o, remainder, and r.
3. Loop over n from 1 to 500
4. Set o = n (store the original number).
5. Set r = 0 (initialize sum of cubes).
6. While o is not 0
7. Get the last digit: remainder = o % 10.
8. Add cube of the digit to r: r = r + (remainder × remainder × remainder).
9. Remove the last digit: o = o / 10.
10. After the loop
11. If r == n, then print that n is an Armstrong number.
12. End.

## PROGRAM
```
#include<stdio.h>
int main(){
    int n,o,remainder,r;
    for(n=1;n<=500;n++){
        o=n;
        r=0;
        while(o!=0){
            remainder=o%10;
            r+=remainder*remainder*remainder;
            o/=10;
        }
        if(r==n){
            printf("%d is a Armstrong number\n",n);
        }
    }
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/31c9fad0-a708-4df9-8b0d-8fe77229065e)







## RESULT
Thus the program to print Armstrong Numbers between 1 and 500 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the elements of an array present on even position

## ALGORITHM
1. Start.
2. Declare integers: n and i.
3. Input an integer n (size of the array).
4. Declare an array a of size n.
5. For i = 0 to n-1
6. Read an integer and store it in a[i].
7. For i = 1 to n-1, incrementing i by 2 each time:
8. Print a[i] (elements at odd indices).
9. End.



## PROGRAM
```
#include <stdio.h>

int main()
{
    int n, i;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
        
    }
    for(i=1;i<n;i=i+2)  
    {
        printf("%d ",a[i]);
}
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/3b991533-10f2-42dd-9cc1-904adc94caef)








## RESULT
Thus the program to read n elements as input and print the elements of an array present on even position has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of negative elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value is lesser than 0 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int counteven(int arr[],int n){
    int count=0;
    for(int i=0;i<n ;i++){
        if(arr[i]<0){
            count++;
        }
    }
    return count;
    
}
int main()
{
    int n;
    scanf("%d",&n);
    int arr[n];
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    int a=counteven(arr,n);
    printf("count  of negative numbers  in array: %d",a);
    
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/1f85dcdd-07b2-40bd-ab26-120c380d09b4)





## RESULT
Thus the program to count total number of negative elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

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
#include<stdio.h>
int main(){
    int a;
    scanf("%d",&a);
    int arr[a];
    for(int i=0;i<a;i++){
        scanf("%d",&arr[i]);
    }
    for(int i=0;i<a;i++){
        if(arr[i]%2==0)
        printf("E ");
        else
        printf("%d ",arr[i]);
    }
    return 0;
}
```

## Output:
 ![image](https://github.com/user-attachments/assets/661f6c53-77e5-499c-a28c-8cf7a52fe155)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



