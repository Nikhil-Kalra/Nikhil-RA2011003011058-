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
         
#### Question 7:
                           
#include <iostream>
using namespace std;
class test{
public:
int my_variable;
};
int main() {
test code_chef;
cin>>code_chef.my_variable;
if(code_chef.my_variable%2==0){
cout<<"Even";
}
else{
cout<<"Odd";
}
return 0;
}

#### Question 8:
 
#include<iostream>
using namespace std;
void printsums(int N)
{
int end;    
int start=1;
end=(N+1)/2; 
int sum=0;
    while(start<end)
    {
    for (int i=start;i<=end;i++)
        {
        sum=+i;
        if (sum == N)
            {
            for (int j=start;j<=i;j++)
            cout<<j<<" ";
            cout<<"/n";
            break;
            }
        if (sum>N)
        break;
        }
    sum=0;
    start++;
    }
}
int main()
{
int n;
cin>>n;
printsums(n);
return 0;
}
  
Question 9:
  
#include <iostream>
#include<climits>
using namespace std;
int main() {
int length;
cout<<"enter the length of the array"<<endl;
cin>>length;
int array[length];
for(int i=0;i<length;i++){
cin>>array[i];
}
int min=array[0];int max=array[0];
for(int i=1;i<length;i++){
if(array[i]>max)
max = array[i];
else if(array[i]<min)
min = array[i];
}
cout<< min<<" "<<max;
return 0;
}

Question 10:
                     
#include <stdio.h>
#include <string.h>
int main()
{
int t,i,diff_count;
scanf("%d",&t);
char s[100001];
while(t--){
diff_count=0;
scanf("%s",s);
for(int i=0;i<strlen(s)-1;i++){
if(s[i]==s[i+1])
diff_count++;
}
printf("%d\n",diff_count);
}
return 0;
}



  
