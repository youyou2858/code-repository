#include <stdio.h>

int main()
{
	int i, num;
	_Bool flag=1;
	
	printf("请输入一个整数，我来判断是不是素数："); 
	scanf("%d",&num);
	for(i=2;i<=num/2;i++) 
	{
		if(num%i==0)
		{
			flag=0;
		}
	}
	if(flag)
	{
		printf("%d是个素数",num);
	}
	else
	{
		printf("%d不是个素数",num);
	}
	return 0;
}
