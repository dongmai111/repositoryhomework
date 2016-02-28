# repositoryhomework



#include <iostream>


#include "LargeIntP.h"
using namespace std;

int main()
{
    LargeIntProject largeInteger;
    cout<<"Enter an extreme large integer (Max: 40 digits)"<<endl;
    cin>>largeInteger;
    cout<<largeInteger<<endl;

    cout<<"Enter two numbers to do addition:"<<endl;
    LargeIntProject x,y;
    cin>>x>>y;
    cout<<x+y<<endl;

    cout<<"The numbers are";
    if(x==y)
    {
        cout<<" equal"<<endl;
    }
    else
    {
        cout<<" not equals"<<endl;
    }


    return 0;
}

