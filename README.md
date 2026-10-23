# -program-to-swap-two-numbers-using-pointers-without-using-another-variable

#include<iostream>
  using namespace std;  
    int main(){
        int x,y;
        cout<<"enter the value of x and y : "<<"\n";
        cin>>x>>y;

        int *p=&x;
        int *q=&y;

        cout<<"before swap : "<<x<<" "<<y<<"\n";

       *p=*p+*q;
       *q=*p-*q;
        *p=*p-*q;

        cout<<"after swap : "<<x<<" "<<y<<"\n";

        return 0;
    }
