**PROGRAM NO 9.1**

#include<iostream>
using namespace std;
void show();
int main()
{
	show();
	return 0;
}
void show()
{
	cout<<"Programming makes life interesting";
}

**PROGRAM N0 9.2**

#include<iostream>
using namespace std;
void max(int a, int b);
int main()
{
	int x,y;
	cout<<"enter two number :";
	cin>>x>>y;
	max(x,y);
	return 0;
}
void max(int a, int b)
{
	if(a>b)
	cout<<"maximun number is "<<a;
	else
	cout<<"maximun number is "<<b;
}

**PROGRAM N0 9.3**

#include<iostream>
using namespace std;
void table(int num);
int main()
{
	int n;
	cout<<"enter a number :";
	cin>>n;
	table(n);
	return 0;
}
void table(int num)
{
	int c;
	for(c=1;c<=10;c++)
	{
		cout<<num<<"*"<<c<<"="<<num*c<<endl;
	}
}

**PROGRAM N0 9.4**

#include<iostream>
using namespace std;
void value(int n);
int main()
{
	int num;
	cout<<"enter number :";
	cin>>num;
	value(num);
	return 0;
}
void value(int n)
{
	int p,s;
	p=n-1;
	s=n+1;
	cout<<"The number before "<<n<<" is "<<p<<endl;
	cout<<"The number after "<<n<<" is "<<s;
}

**PROGRAM N0 9.5**

#include<iostream>
using namespace std;
void factorial(int n);
int main()
{
	int num;
	cout<<"enter number :";
	cin>>num;
	factorial(num);
	return 0;
}
void factorial(int n)
{
	int i;
	long f=1;
	for(i=1;i<=n;i++)
	{
		f=f*i;
	}
	cout<<"The factorial of "<<n<<" is "<<f;
}

**PROGRAM N0 9.6**

#include<iostream>
using namespace std;
void num_chk(int n)

{
	int c=0,i;
	for(i=2;i<n;i++)
	{
		if(n%i==0)
		c=1;
	}
	if(n%2==0&&c==0)
	cout<<n<<" is prime even number";
	else if(n%2!=0&&c==0)
	cout<<n<<" is prime odd number";
	else if(n%2==0&&c==1)
	cout<<n<<" is even number not prime number";
	else if(n%2!=0&&c==1)
	cout<<n<<" is odd number not prime number";
	else
	cout<<n<<" is prime even number";
}
int main()
{
	int n;
	cout<<"Enter a number :";
	cin>>n;
	cout<<"\n-------------------------";
	cout<<"\n| Nature of number is |\n";
	cout<<"-------------------------\n";
	num_chk(n);
	return 0;
}

**PROGRAM N0 9.7**

#include<iostream>
using namespace std;
void cal(int a,int b, char c);
int main()
{
	int x,y;
	char op;
	cout<<"enter 1st number , operator , 2nd number : ";
	cin>>x>>op>>y;
	cal(x,y,op);
	return 0;
}
void cal(int a,int b, char c)
{
	switch(c)
	{
		case '+':
			cout<<a<<"+"<<b<<"="<<a+b;
			break;
		case '-':
			cout<<a<<"-"<<b<<"="<<a-b;
			break;
		case '*':
			cout<<a<<"*"<<b<<"="<<a*b;
			break;	
		case '/':
			if(b==0)
			cout<<"invalid number";
			else
			cout<<a<<"/"<<b<<"="<<a/b;
			break;	
		case '%':
			cout<<a<<"%"<<b<<"="<<a%b;
			break;	
		default:
			cout<<"invalid number";
	}
}

**PROGRAM N0 9.8**

#include<iostream>
using namespace std;
void shape(int, char);
int main()
{
	int num;
	char ch;
	cout<<"enter a number : ";
	cin>>num;
	cout<<"enter a character : ";
	cin>>ch;
	shape(num,ch);
	return 0;
}
void shape(int n, char c)
{
	int i,j;
	for(i=1;i<=n;i++)
	{
	    cout<<endl;
		for(j=1;j<=n;j++)
		cout<<c;
	}
}

**PROGRAM N0 9.9**

#include<iostream>
using namespace std;
void swap(int &x, char &y);
int main()
{
	int a,b;
	cout<<"enter two integers :";
	cin>>a>>b;
	cout<<"Values before swapping are:\n";
	cout<<"a= "<<a<<"\nb= "<<b<<endl;
	swap(a,b);
	cout<<"Values after swapping are:\n"; 
	cout<<"a= "<<a<<"\nb= "<<b<<endl;
	return 0;
}
void swap(int &x, char &y)
{
	int temp;
	temp=x;
	x=y;
	y=temp;
}

**PROGRAM N0 9.10**

#include<iostream>
using namespace std;
char grade(int x);
int main()
{
	int marks;
	char g;
	cout<<"Enter marks :";
	cin>>marks;
	g=grade(marks);
	cout<<"Your grade is "<<g;
	return 0;
}
char grade(int x)
{
	if(x>80)
	return 'A';
	else if(x>60)
	return 'B';
	else if(x>40)
	return 'C';
	else
	return 'F';
}

**PROGRAM N0 9.11**

#include<iostream>
using namespace std;
int mul(int,int);
int main()
{
	int i,r,x,y;
	for(i=1;i<=5;i++)
	{
		cout<<"Enter pair of integers: ";
		cin>>x>>y;
		r=mul(x,y);
		if(r==1)
		cout<<y<<" is multiple of "<<x<<endl;
		else
		cout<<y<<" is not multiple of "<<x<<endl;
	}	
	return 0;
}
int mul(int a,int b)
{
	if(b%a==0)
	return 1;
	else
	return 0;
}

**PROGRAM N0 9.12**

#include<iostream>
using namespace std;
float area(int b,int h);
int main()
{
	int base,height;
	float a;
	cout<<"Enter base & height: ";
	cin>>base>>height;
	a=area(base,height);
	cout<<"Area of Triangle = "<<a;
	return 0;
}
float area(int b,int h)
{
	float ar;
	ar=0.5*b*h;
	return ar;
}

**PROGRAM N0 9.13**

