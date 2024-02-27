#include<iostream>
#include<stdlib.h>
using namespace std;

void swap(int *a,int *b);
int main()
{
 int a,b;
 cin>>a>>b;
 swap(a,b);
 cout<<a<<' '<<b;
}

//swap函数只负责交换变量的值，不能输出交换后的结果
void swap(int *a,int *b)
{
 int *p;
 p=a;
 a=b;
 b=p;
 free(p);
}
