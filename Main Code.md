//# Basic-Calculator-
//basic calculator using c++
#include<iostream>
using namespace std;
int main(){

   float num1,num2;
   char op;
   cout<<"Welcome to the calculator"<<endl;
   cout<<"Enter num1:"<<endl;
   cin>>num1;
   cout<<"Enter num2:"<<endl;
   cin>>num2;
   cout<<"Choose your operator'+,-,*,/'"<<endl;
   cin>>op;
   switch (op)
   {
   case '+':
   cout<<num1<<op<<num2<<"="<<num1+num2;
    break;
   
   case '-':
   if (num1>num2)
   {
    cout<<num1<<op<<num2<<"="<<num1-num2;
   }
   else
   cout<<num2<<op<<num1<<"="<<num2-num1;
   break;
   
   case '*':
   cout<<num1<<op<<num2<<"="<<num1*num2;
   break;

   case '/':
   if (num2==0.0)
   {
    cout<<"Not Defined";
   }
   
   cout<<num1<<op<<num2<<"="<<num1/num2;
   break;

   
   default:
   cout<<"Invalid Operator";
   
   }


}
