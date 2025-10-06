































#include <stdio.h>
int main()
{
    char n[30];
    char p[30];
    char d[10];
    int q;
    int rate;
    int i;
    int j;
    int total=0;
    int amount=0;
    printf("\t\t\t\t\tPLYWOOD SHOP\n\n");
    printf("GSTIN:XXXXXX\t\t\t\t\t\t\t");
    printf("Date:");
    
    scanf("%s",&d);
    printf("---------------------------------------------------------------------------\n");
    printf("Name of customer:");
    scanf("%s",&n);
    printf("Number of items:");
    scanf("%d",&i);
    printf("\n\t\tParticulars\t\t\tRate\t\t\t\tQTY");
    for(j=1;j<=i;j++)
    {
        printf("\n%d).",j);
    scanf("\t\t%s\t\t\t%d\t\t\t\t%d",&p,&rate,&q);
    amount=rate*q;
    total+=amount;
    }
    printf("\nTotal is:%d",total);
    printf("\nGST=18per");
    float gr=total+(0.18*total);
    printf("\n\nGrand total is:%f",gr);
    printf("\n------------------------------------------------------------------------------\n");
    printf("THANKS FOR SHOPPING");
}

