# programming
程序设计
//冒泡排序
#include<stdio.h>
int main()
{
	int n,i,j,k,t;
	scanf("%d",&n);
	int a[n];
	for(i=0;i<n;i++)
		scanf("%d",&a[i]);
	for(i=0;i<n-1;i++)
	{
		int k=1;
		for(j=0;j<n-i-1;j++)
		{
			if(a[j]>a[j+1])
			{
				t=a[j];
				a[j]=a[j+1];
				a[j+1]=t;
				k=0;
			}
		}
		if(k)
			break;
	}
	for(i=0;i<n;i++)
		printf("%d ",a[i]);
} 
void sort(int a[],int n)
{
	int i,j,k,t;
		for(i=0;i<n-1;i++)
	{
		for(j=0;j<n-i-1;j++)
		{
			if(a[j]>a[j+1])
			{
				t=a[j];
				a[j]=a[j+1];
				a[j+1]=t;
				k=0;
			}
		}
		if(k)
			break;
	}
}
