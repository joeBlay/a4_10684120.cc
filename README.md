//c++ program that uses recursion to find the GCD of two numbers
#include<iostream>
using namespace std;

int gcd(int x, int y);

int main()
{
   int x,y;

   cout << "Enter the first integer:";
   cin>>x;
   cout<<"Enter the second integer:";
   cin >>y;

    cout << "GCD of x and y is:"<< gcd(x,y);

   return 0;
}

int gcd(int x, int y)
{
    if (y != 0)
       return gcd(y,x%y);
    else
       return y;
}
