
----------
## **Assignment No : 01**

## **Assignment Name : SWITCH STATEMENT**

## **Submission Date : 05 November 2024**

----------



## **Code :**
```C
#include <stdio.h>
int main()
{
    int choice;
    double balance=0.0, amount;

    while (1){
printf("\nBanking System Menu:\n");
printf("1. Deposite\n");
printf("2. Withdraw\n");
printf("3. Balance Inquiry\n");
printf("4. Exit\n");
printf("Enter your choice: ");
scanf("%d",&choice);


switch (choice) {
case 1:
printf("Enter the amount to deposite: ");
scanf("%lf",&amount);
if(amount < 0){printf("Error: Check the Amount");}
else{
balance=balance+amount;
printf("Your deposite is successful. Thank You.");
}
break;


case 2:
printf("Enter the amount to Withdraw: ");
scanf("%lf",&amount);
if(amount < 0){printf("Error: Check the Amount");}
else if(amount>balance){printf("Error: You have not enough money in your account.");}
else{
balance=balance-amount;
printf("Your Withdraw is successful. Thank You.");
}
break;


case 3:

printf("Your Balance is: %.2lf\n",balance);
printf("Thank You");
break;


case 4:
printf("Thank you for using this banking system. Have a great day!\n");
return 0;


default:
printf("Error: Please Check the description of Menu");


}


    }
}

## **Output :**
<p align="center">
(https://github.com/user-attachments/assets/c7b5a016-eda9-4aa2-a2ec-2b1402d764d3
</p>

## **Discussion :**
<div align="justify">
Input and Output : scanf to take two integer inputs and printf to display the result.<br>
Arithmetic Operation : A simple addition operation using the variables a and b.<br>
Format Specifiers : %d handle integer values for both input and output.<br>
</div>

## **Conclusion :**
<div align="justify">
The program effectively shows output “hello world”<br>
</div>