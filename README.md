# qwer888
#include <stdio.h>
 
int main(int argc, char *argv[])
{
    int R,C,n;
    scanf("%d",&R);
    scanf("%d",&C); 
    scanf("%d",&n);
    int a[n];
    int i=0;
    while(i<n)
    {
      scanf("%d",&a[i]);  
      i++;
    }
    i=0;
    while(i<n)
    {
        int b=a[i]-1;
        printf("%d  ",b/C+1);
        if((b/C+1)%2==0) 
            printf("%d\n",C-b%C);
        else
            printf("%d\n",b%C+1);
        i++;
    }
    return 0;
}
