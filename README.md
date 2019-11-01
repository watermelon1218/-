#include<stdio.h>
#define N 10
int main()
{
   int i, j, temp;
   int a[N];
   for(i=0;i<N;i++)
   {
      scanf("%d",&a[i]);
    }
   for(i=0;i<N-1;i++)
   {
         for(j=0;j<N-1-i;j++)
         {
             if(a[j]>a[j+1])
             {
                 temp=a[j];
                 a[j]=a[j+1];
                 a[j+1]=temp;
               }
          }
     }
     for(i=0;i<N;i++)
     {
          printf("%d",a[i]);
     }
     return 0;
  }
