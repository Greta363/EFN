# EFN

#include <iostream>
using namespace std;
int main()
 {
  int n=4000000,sum=0;
  long long a[1000000];
  a[0]=0;
  a[1]=1;
  for(int i=2; i<=n; i++)
  {
   a[i]=a[i-1]+a[i-2];
  }
  for(int i=2; i<=n; i++)
   if(a[i]%2==0)
   {
   sum=sum+a[i];
   }
  cout<<sum;
}
