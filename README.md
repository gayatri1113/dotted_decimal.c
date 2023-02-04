//# dotted_decimal.c//
#include<stdio.h>
int main()
{
    int a,b,c,d;
    printf("enter the first byte\n");
    scanf("%d",&a);
    printf("enter the second byte\n");
    scanf("%d",&b);
    printf("enter the third byte\n");
    scanf("%d",&c);
    printf("enter the forth byte\n");
    scanf("%d",&d);
    if(a<=255&& b<=255&& c<=255&& d<=255)
    {
        printf("the IP address is %d.%d.%d.%d\n",a,b,c,d);
    }
    else
    {
        printf("invalid IP");
    }
    if(a<=127)
    {
        printf("Class A\n");
    }
    else if(a>127&&a<=191)
    {
        printf("Class B\n");
    }
    else if(a>191&&a<=223)
    {
        printf("Class C\n");
    }
    else if(a>223&&a<=239)
    {
        printf("Class D\n");
    }
    else
    {
        printf("Class E\n");
    }
return 0;
}
