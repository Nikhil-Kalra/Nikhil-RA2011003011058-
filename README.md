solutions
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
  
#### Question 9:
  
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

#### Question 10:
                     
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
                                
### Task 2: Solve the given programs:
      
#### Question 1:

#include<stdio.h>
#include<string.h>
int main(){
    char arr[1000][50];
    int s,j;
    char temp[50];
    scanf("%d",&s);
    for (int i=0;i<s;i++){
        scanf("%s",arr[i]);
        int len=strlen(arr[i]);
        if(len<4){
            arr[i][3]=arr[i][len-1];
        }
    }
    for(int i=0;i<s;i++){
        for (int j=i+1;j<s;j++){
            if (arr[i][3]>arr[j][3]){
                strcpy(temp,arr[i]);
                strcpy(arr[i],arr[j]);
                strcpy(arr[j],temp);
            }
        }
    }
    for(int i=0;i<s;i++){
        printf("%s\n",arr[i]);
    }
    return 0;
}
                                
                                
#### Question 2:
                                
#include <iostream>
using namespace std;

int kthSmallest(int arr[], int n, int k)
{
for(int i=0;i<=n-2;i++){
		for(int j=0;j<=n-2-i;j++){
			if(arr[j]>arr[j+1]){
			    int temp=arr[j];
			    arr[j]=arr[j+1];
			    arr[j+1]=temp;
			}
		}
}
return arr[k-1];
}

int main()
{
    int prime=0;
	int arr[] = { 7,10,4,5,2 };
	int n = sizeof(arr) / sizeof(arr[0]), k = 4;
    kthSmallest(arr, n, k);
    cout<<arr[k-1]<<" ";
    cout<<"and"<<" ";
    for(int i=2;i<arr[k-1]/2;i++){
        if(arr[k-1]%i==0){
            prime=0;
            break;
        }
        else{
            prime=1;
        }
    }
    if(prime==1){
        cout<<arr[k-1]<<" "<<"is prime";
    }
    else{
        cout<<arr[k-1]<<" "<<"is not prime";
    }
	return 0;
}
  
#### Question 3:

#include<iostream>
using namespace std;
int main(){
    int n=26;
    int token=0;
    for (int i=0;i<n;i++){
        if (token==0){
            cout<<(char)(i+65)<<endl;
            token=1;
        }
        else if(token==1){
            token=2;
        }
        else if(token==2){
            cout<<(char)(i+97)<<endl;
            token=3;
        }
        else if(token==3){
            token=0;
        }
    }
    return 0;
}

#### Question 4:
                              
#include<stdio.h>
#include<math.h>
int main(){
    int n,count=0,id,num1,num2;
    float done=0.0;
    scanf("%d",&n);
    int n1=n*n;
    int n2=n1;
    printf("%d,%d\n",n1,n2);
    while(n1!=0){
        n1=n1/10;
        count++;
    }
    count--;
    n1=n2;
    if(n1%2==0){
        id=count/2;
    }
    else{
        id=count/2+1;
    }
    for(int i=0;i<id;i++){
        num1+=(n1%10)*(int)(pow(10.0,done));
        done+=1.0;
        n1=n1/10;
    }
    if(num1+n1!=n){
        printf("Not Chef Number");
    }
    else{
        printf("Chef Number");
    }
return 0;
}
  

   



  
