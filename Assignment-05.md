
----------
## **Assignment No : 05**

## **Assignment Name : Structure**

## **Submission Date : 17 January 2025**

----------



## **Code :**
```C
#include <stdio.h>
#include <string.h>

struct student {
    char name[20];
    int roll;
    int age;
    char dep[4];
    float cgpa;
};

int main() {
    struct student s[10];

    strcpy(s[0].name, "Fahad"); s[0].roll = 1; s[0].age = 20; strcpy(s[0].dep, "CSE"); s[0].cgpa = 3.5;
    strcpy(s[1].name, "Mahir"); s[1].roll = 2; s[1].age = 21; strcpy(s[1].dep, "ECE"); s[1].cgpa = 3.8;
    strcpy(s[2].name, "Arif");  s[2].roll = 3; s[2].age = 19; strcpy(s[2].dep, "EEE"); s[2].cgpa = 3.6;
    strcpy(s[3].name, "Sakib"); s[3].roll = 4; s[3].age = 22; strcpy(s[3].dep, "ME");  s[3].cgpa = 3.7;
    strcpy(s[4].name, "Rakib"); s[4].roll = 5; s[4].age = 20; strcpy(s[4].dep, "CE");  s[4].cgpa = 3.4;
    strcpy(s[5].name, "Parvej");s[5].roll = 6; s[5].age = 21; strcpy(s[5].dep, "CSE"); s[5].cgpa = 3.9;
    strcpy(s[6].name, "kafi");  s[6].roll = 7; s[6].age = 19; strcpy(s[6].dep, "ECE"); s[6].cgpa = 3.6;
    strcpy(s[7].name, "Nahid"); s[7].roll = 8; s[7].age = 22; strcpy(s[7].dep, "EEE"); s[7].cgpa = 3.5;
    strcpy(s[8].name, "Ali");   s[8].roll = 9; s[8].age = 20; strcpy(s[8].dep, "ME");  s[8].cgpa = 3.3;
    strcpy(s[9].name, "Robin"); s[9].roll = 10;s[9].age = 21; strcpy(s[9].dep, "CE");  s[9].cgpa = 3.8;

    printf("Student names in the specified order:\n");
    

    for (int i = 0; i <= 9; i++) {
        printf("%s\n", s[i].name);
    }

    return 0;
}


```

## **Output :**
<p align="center">
<img src = "https://github.com/user-attachments/assets/bfc9f9ab-cdba-4597-94d9-ad64594c5ac2">
</p>


