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
