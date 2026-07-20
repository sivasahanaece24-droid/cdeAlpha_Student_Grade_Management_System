#include <stdio.h>

int main()
{
    char name[50];
    int m1, m2, m3, total;
    float average;
    char grade;

    printf("Enter Student Name: ");
    scanf("%s", name);

    printf("Enter Mark 1: ");
    scanf("%d", &m1);

    printf("Enter Mark 2: ");
    scanf("%d", &m2);

    printf("Enter Mark 3: ");
    scanf("%d", &m3);

    total = m1 + m2 + m3;
    average = total / 3.0;

    if (average >= 90)
        grade = 'A';
    else if (average >= 75)
        grade = 'B';
    else if (average >= 60)
        grade = 'C';
    else if (average >= 40)
        grade = 'D';
    else
        grade = 'F';

    printf("\n----- Student Report -----\n");
    printf("Student Name : %s\n", name);
    printf("Total Marks  : %d\n", total);
    printf("Average      : %.2f\n", average);
    printf("Grade        : %c\n", grade);

    return 0;
}
