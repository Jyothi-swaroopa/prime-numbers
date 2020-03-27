# prime-numbers

#include <iostream>

#include <conio.h>

#include <iomanip>

#include <math.h>

using namespace std;

int main()

{

    int a,b;

    int i,j,flat=0,cnt=0;

    cout<<"Enter first number of the range"<<endl;

    cin>>a;

    cout<<"Enter second number of the range"<<endl;

    cin>>b;

    cout<<"Prime numbers b/w"<<a<<"&"<<b<<"are"<<endl;

    for(i=a;i<=b;i++)

    {

        for(j=2;j<=sqrt(i);j++)

        {

            if(i%j==0)

            {

                flat++;

            }

        }

       if(flat==0&&i!=1)

       {

           cnt++;

           cout<<"Prime number is "<<i<<endl;

           flat=0;

       }

       flat=0;

    }

    cout<<"Total prime number b/w"<<a<<"&"<<b<<"are"<<cnt<<endl;

    return 1;

}

 

