
----------
## **Assignment No : 04 (A)**

## **Assignment Name : Computing Interest**

## **Submission Date : 28 November 2024**

----------

## **Code : (Using While Loop)**
```C
#include <stdio.h>
int main()
{
    //declearation
    int ir,year;
    int arr_ir[5];
    float arr[5];
    //input
    printf("Enter interest rate:");
    scanf("%d",&ir);

    printf("Enter number of years:");
    scanf("%d",&year);  
//row of %(intarest)
for (int i=0; i<5; i++)
{
arr_ir[i]=ir;
ir++;
arr[i]=100;
}
//column of Year
    printf("Years\t"); for (int i=0; i<5; i++){printf("\t%d%%\t",arr_ir[i]);}

    printf("\n");

//row of data

    for (int i=1; i<=year; i++)
    {
printf("  %d\t ",i);
for (int j=0; j<5; j++)
{
printf("     %.2f\t ",arr[j]+arr[j]*arr_ir[j]*0.01);
}

//logic for compound interest

for (int j=0; j<5; j++){
arr[j]=arr[j]+arr[j]*arr_ir[j]*0.01;
}

printf("\n");


    }
}
```

## **Output :**
<p align="center">
<img src = "https://github.com/user-attachments/assets/fdc4b2ac-8e25-44f6-a61e-ee318718cb27">
</p>


----------


## **Assignment No : 4 (B)**

## **Assignment Name : Effect of Call by Value**

## **Submission Date : 28 November 2024**

----------

## **Code : **
```C
#include <stdio.h>
int func(int x);
int main()
{
int a;
a=3;

printf("The value of a before function call: %d\n",a);

func(a);

printf("The value of a afrer function call: %d\n",a);

printf("The value of x in the function: %d\n",func(a));

}

int func(int x)
{
    return x=x+10;
}

```

## **Discussion :**
<div align="justify">
 
This code shows how Call by Value works. In the main() function, the variable a is set to 3. When func(a) is called, only a copy of a is sent to the function func. Inside the function, the parameter x gets this copy and adds 10 to it. However, this change happens only to the copy, so the original a in main() stays the same.

After the function call, a is still 3 in main(), but the function returns the modified value of x (which is 13). This shows that changes made in the function do not affect the original variable in main() because only a copy was passed.

## **Output :**
<p align="center">
<img src = "https://github.com/user-attachments/assets/19b0d711-bc9c-4035-a229-6d112afaf3ca">
</p>
