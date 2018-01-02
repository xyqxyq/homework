#include <iostream>
using namespace std;
int main()
{
	cout<<"**************************************************"<<endl;
	cout<<"***************** 小小计算器 *********************"<<endl;
	cout<<"*****************   1.加法   *********************"<<endl;
	cout<<"*****************   2.减法   *********************"<<endl;
	cout<<"*****************   3.乘法   *********************"<<endl;
	cout<<"*****************   4.除法   *********************"<<endl;
	cout<<"*****************   5.圆的面积   *****************"<<endl;
	cout<<"*****************   6.字母的大小写转换   *********"<<endl;
	cout<<"*****************   7.列出所有奇数   *************"<<endl;
	cout<<"*****************   8.求所有奇数的和   ***********"<<endl;
	cout<<"**************************************************"<<endl;
	cout<<"请输入三个数,进行1到5的运算，每个数以空格结束"<<endl;
	int a,b,add,sub,mul,div,r;
	double s;
	cin>>a>>b>>r;
	const PI=3.14;
	add=a+b;
	sub=a-b;
	mul=a*b;
	div=a/b;
	s=PI*r*r;
	cout<<"加:"<<add<<endl;
	cout<<"减:"<<sub<<endl;
	cout<<"乘:"<<mul<<endl;
	cout<<"除:"<<div<<endl;
	cout<<"面积:"<<s<<endl;
	cout<<endl;
	cout<<"请输入字母，可进行大小写转换"<<endl;
	char ch;
	cin>>ch;
	if (ch>=65&&ch<=90)
	{
		ch=ch+32;
		cout<<ch<<endl;
	}
	else if(ch>=97&&ch<=122)
	{
		ch=ch-32;
		cout<<ch<<endl;
	}
	else
		cout<<"输入非法"<<endl;
	cout<<endl;
	cout<<"请输入两个数比较他们的大小，每个数以空格结束"<<endl;
	float num1,num2;
	cin>>num1>>num2;
	if (num1>=num2)
		cout<<num1<<endl;
	else
		cout<<num2<<endl;
	cout<<endl;
	cout<<"循环一：请输入一个二百以内的整数，可找出从零到该数中的所有奇数，并求和"<<endl;
	int t=0,num3;
	cin>>num3;
	for (int i=1;i<=num3;i+=2)
	{
		cout<<i<<" ";
		t+=i;
	}
		cout<<endl;
		cout<<"求和结果："<<t<<endl;
	cout<<endl;
	cout<<"循环二：请输入一个二百以内的整数，可找出从零到该数中的所有奇数，并求和"<<endl;
	int j=1,k=0;
	while (j<=num3)
	{
		cout<<j<<" ";
		k+=j;
		j+=2;

	}
		cout<<endl;
		cout<<"求和结果："<<k<<endl;
	cout<<endl;
	cout<<"循环三：请输入一个二百以内的整数，可找出从零到该数中的所有奇数，并求和"<<endl;
	{
		int l=1,m=0;
		do
		{
			cout<<l<<" ";
			m+=l;
			l+=2;
		}while (l<=num3);
		cout<<endl;
		cout<<"求和结果："<<m<<endl;
	}
	return 0;
}
