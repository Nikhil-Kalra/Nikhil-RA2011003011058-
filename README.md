# solutions
## Task for 2nd year students
### Task 1: Spot the error in following questions:

#### Question 1:

#include <stdio.h>
void main()
{
int number, LD;
printf(" Enter a number");
scanf("%d",&number);
LD = number / 10;
printf(" \n The Last Digit of a Given Number %d = %d", number,LD);
return 0;
}

#### Question 2:

int main(int len, int* arr, int value)
{
int sum = 0;
for(int i =0 ; i< len-1; i++ )
{
if(arr[i]%value == 0)
sum =+ arr[i];
sum=0;
}
return sum;
}

#### Question 3:

#include <stdio.h>
int main()
{
for(int i=1;i<=4;i--)
{
for(int j=1;j<=4;j++)
{
if(i != j)
{
printf("*");
}
else
{
printf(" ");
}
}
printf("\n");
}
return 0;
}

#### Question 4:

#include <stdio.h>
int main() {
char a='A';
a>10?printf("Yes"):printf("No");
return 0;
}

#### Question 5:

#include <iostream>
using namespace std;
int main() {
int o,i,s;
for(o=5; o>=1;o--)
{
for(s=1;s<=5-o;s++){
cout<<" ";
for (i=1;i<=o;i++){
cout<<"*";}
cout<<endl;
}}
return 0;
}

#### Question 6:
  
#include<stdio.h>
int main()
{
    int z;
    printf("Enter a number: ");
    scanf("%d",&z);
    for (int i=0;i<9;i++){
        if(z==i){
            printf("They are equal\n");
        }
        else{
            printf("They are not equal\n");
        }
    }
    return 0;
}

  
