**题目:**

![题目图片](https://github.com/lllllliuxt/acmer/blob/master/%E5%8C%97%E9%82%AE%E6%9C%BA%E8%AF%95/%E9%A2%98%E7%9B%AE.png)

**代码:**
# 经验
- 输出的大小写要注意一致
- scanf的格式化输入启发很大，节省很多
- while（T--）
- sscanf()的使用
```C++
#include <iostream>
#include <cstdio>
#include <cstring>
using namespace std;

int main()
{
	int ip[4],T;
	char buf[20],k;
	bool flag;
	int count;
	scanf("%d",&T);
	while(T--)
	{
		flag=true;
		scanf("%s",buf);
		count=sscanf(buf,"%d.%d.%d.%d%c",&ip[0],&ip[1],&ip[2],&ip[3],&k);
		if(count!=4)//输入的个数为4，没有废串 ，若中间有字符串则停止输入 
		{
			flag=false;
		} 
		else
		for(int i=0;i<4;++i)
			{
				if(ip[i]>255||ip[i]<0)
					{
						flag=false;
						break;
					}
			}
			
		printf("%s\n",flag?"Yes":"No");
	}
	return 0;
}
```
