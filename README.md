#include<stdio.h>
int main()
{
    int t,n,i,min=10000000000,k;
    scanf("%d",&t);
    while(t--)
    {
     min=10000000000;
     scanf("%d%d",&n,&k);
     int a[n];
     for(i=0;i<n;i++)
     {
      scanf("%d",&a[i]);
      if(a[i]<min)
       min=a[i];
     }
     //printf("%d ",min);
     if(min>=k)
      printf("0\n");
     else
      printf("%d\n",k-min);
    }
    return 0;

}
