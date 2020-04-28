#include <stdio.h>

int main()
{
    int n;
    printf("enter the number\n");
    scanf("%d",&n);
    printf("sum of digits is\n");
    printf("%d",sum(n));
}

int sum(n)
{
    if(n==0)
    {
        return 0;
    }
    return(n%10 + sum(n/10));
}
