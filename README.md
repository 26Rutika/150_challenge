# 150_challenge
1. Check if number is even or odd
   (without using % operator)
   //Check even or odd
    #include<iostream>
    using namespace std;
    bool isEven(int n)
   {
	return(!(n&1));
   }
   int main()
 {
	int n;
	cin>>n;
	int a=isEven(n);
	if(a)
	{
		cout<<"\nEven";
	}
	else
	{
		cout<<"\nodd";
	}
}
2.
 #include<iostream>
 #include<math.h>
 using namespace std;
 int  isPrime(int n)
 {
 int count=0;
 for(int i=1;i<=sqrt(n);i++)	
 {
	if(n%i==0)
	{
	  count++;	
	
	if(n/i!=i)
	{
		count++;	
	}
  }
 }
 return count;
 }
 int main()
 {
 int n;
 cin>>n;
 int a=isPrime(n);
 if(a>2)
 {
	cout<<"\nNumber is not prime";
 }
 else
 {
	cout<<"\nNumber is prime";
 }	
}
3.Armstrong number
#include<iostream>
using namespace std;
bool isArmstrong(int n)
{
	int temp=n,rev;
	while(n>0)
	{
		int l=n%10;
		rev=rev+(l*l*l);
		n=n/10;
	}
	if(temp==rev)
	{
		return 1;
	}
	else
	{
		return 0;
	}
}
int main()
{
int n;
cin>>n;
int a=isArmstrong(n);
cout<<a;
}
