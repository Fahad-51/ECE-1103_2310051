
----------
## **Assignment No : 03**

## **Assignment Name : Check The Matched Number**

## **Submission Date : 20 November 2024**

----------



## **Code :**
```C
#include <stdio.h>
int main()
{
int n;
printf("Enter the number of Data: ");
scanf("%d",&n);
int arr[n];
printf("Enter The Data: ");

for( int i=0; i<n; i++){scanf("%d",&arr[i]);}


for ( int i=0; i<n; i++)
{
    for ( int j=0; j<n; j++){if(arr[i]==arr[j] && i!=j){printf("Same number found which is: %d in index %d & %d.",arr[i],i,j); return 0;}}
}
printf("No value has matched!");
}

```

## **Output :**
<p align="center">
<img src = "https://github.com/user-attachments/assets/44945641-8eb0-49ef-a6cd-5790d55f1758">
</p>

