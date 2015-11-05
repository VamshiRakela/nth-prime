Program to find the Nth prime number

#include<stdio.h>
    
int main()
{
     long  int num = 1, ctr, cmr, i, c=1,nn;

    scanf("%lu", &nn);
    while (c <= nn)
    {
        ctr = 0;
        for (i = 1; i <= num; i++)
        {
            if (num%i == 0)
                ctr++;
        }
        if (ctr == 2)
        {
            c++;
            cmr = num;
            
        }
        num++;
    }
    printf("%lu", cmr);
    
    return(0);
}
