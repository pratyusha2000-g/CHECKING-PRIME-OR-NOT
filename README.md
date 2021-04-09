#include<stdio.h>
void prime(int n,int i,int c);
void main()
{
  int n;
  printf("Enter a number \n");
  scanf("%d",&n);
  prime(n,2,0);
}

void prime(int n,int i,int c)
{
  if(i<=n/2)
    {
       if(n%i==0)
           c++;
        i++;
        prime(n,i,c);
     }
   else
    {
       if(c>=1)
         printf("%d is not a prime number",n);
       else
         printf("%d is a prime number",n);
    }
}
       
