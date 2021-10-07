#include <bits/stdc++.h>
using namespace std;
int main()
{
         int t;
         cin>>t;

     while(t--)
    {
         int a,b,c,d;
         cin>>a>>b>>c>>d;
        
         int count=1; int num=0;
         for(int i=0;i<3;i++)
         {
                if(a+b+c<=d){
               cout<<"1"<<endl;
               break;  }
               else if(a+b+c-a<=d ){
                 count++;
                 cout<<count<<endl;
                 break;} 
                else if(a+b+c-b<=d ){
                 count++;
                 cout<<count<<endl;
                 break;} 
                else if(a+b+c-c<=d ){
                 count++;
                 cout<<count<<endl;
                 break;} 
             else{
                 num++;}
                 
        }
            if(num>=3){
             cout<<num<<endl;}
    }
 
    return 0;
}
