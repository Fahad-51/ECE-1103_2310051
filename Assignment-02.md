
----------
## **Assignment No : 02**

## **Assignment Name : Guess the Secret Number with Limited Attempts**

## **Submission Date : 06 November 2024**

----------



## **Code :**
```C
#include <stdio.h>
int main()
{
    int secret_number,range,attempt,total;
    printf("Welcome to \"Guess The Number\"\n");
    printf("Enter the Range: ");
       scanf("%d",&range);
    printf("Enter the Attempt: ");
       scanf("%d",&attempt);
    total=attempt;
    srand(time(0));
    secret_number=rand()%range+1;
    
  
 while(1){


if(attempt==0){printf("Game Over! Your have used all your attempts. Better luck next time!\nThe correct number was: %d",secret_number);return 0;}

else if(attempt>0){

    int guess;
    printf("Guess the number: ");
    scanf("%d",&guess);


    if(guess<secret_number){printf("Opps! The number is small. Try a higher number.\n"); attempt--;}
    else if(guess>secret_number){printf("Opps! The number is large. Try a lower number.\n"); attempt--;}
    else if(guess==secret_number){printf("Congratulations! You guessed the correct number.\nYour score is: %d out of %d",attempt,total);return 0;}
    
  }
}
}

```

## **Output :**
<p align="center">
<img alt="Screenshot 2024-09-16 at 4 00 16 PM" src="https://github.com/user-attachments/assets/17e17ce1-ea24-4ada-9284-e405b41f72a8">
</p>

