#include <stdio.h>
#include <iostream>
#include <string>
using namespace std;

int change(string str)//16进制转十进制 
{
	int sum=0;
	//去除首部的0
	int i;
	while(str[i]=='0')
	{
		str.erase(0,1);
		i++;
	 } 
	 //转化为10进制 
	int n=str.size();
	int tmp;
	int a;
	for(i=0;i<n;++i)
	{
		if(str[i]>='0'&&str[i]<='9')
		{
			a=str[i]-'0';
		}
		else if(str[i]>='a'&&str[i]<='f')
		{
			a=str[i]-'a'+10;
		}
		sum=(sum*16+a);
	}
	return sum;
}

int main()
{
	int n;
	while(scanf("%d",&n)!=EOF)
	{
		getchar();
		for(int i=0;i<n;++i)
		{
			char a[300];
			gets(a);
			string str=a;
			for(int j=2;j<str.size();)
			{
				str.erase(j,1);
				j+=2;
			}//删除空格
			//求总长度 
			int lenth;
			string sub=str.substr(4,4);
			lenth=change(sub);
			//求ip 
			int ip1[4];
			for(int j=0;j<4;++j)
			{
			sub=str.substr(24+2*j,2);
			ip1[j]=change(sub);
			}
			int ip2[4];
	    	for(int j=0;j<4;++j)
			{
			sub=str.substr(32+2*j,2);
			ip2[j]=change(sub);
			}
			//求端口 
			sub=str.substr(1,1);
			int headlen=8*change(sub);
			int port1;
			sub=str.substr(headlen,4);
			port1=change(sub);
			int port2;
			sub=str.substr(headlen+4,4);
			port2=change(sub);
			//输出
			cout <<"Case #"<<i+1<<endl;
			cout <<"Total length = "<<lenth<<" bytes"<<endl;
			cout <<"Source = "<<ip1[0]<<"."<<ip1[1]<<"."<<ip1[2]<<"."<<ip1[3]<<endl;
			cout <<"Destination = "<<ip2[0]<<"."<<ip2[1]<<"."<<ip2[2]<<"."<<ip2[3]<<endl;
			cout <<"Source Port = "<<port1<<endl;
			cout <<"Destination Port = "<<port2<<endl;
			cout << endl;
		}
	}
}
