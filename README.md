#A simple c++ code to print out prime numbers less than a number.

#include <iostream>
#include <conio.h>
using namespace std;

int main()
{
   int n;
   cout<<"Enter a positive number:";
   cin>>n;

   if(n<2){
   cout<<"Invalid Entry...";
   getch();

}

  for(int x=2; x<n; x++){
    int flag=0;
    for(int i=2; i<=x/2; i++){
     if(x%i==0){
       flag=1; break;
}
}
     if(flag==0) cout<<x<<" ";
}
	getch();
	return 0;
}
