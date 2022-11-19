#include<stdio.h>
#include<math.h>
int isprime(int x);
int main()
{
	int x;
	scanf("%d",&x);
	if(isprime(x))
	printf("yes");
	else 
	printf("no");
	
} 
int isprime(int x)
{
	int ret=1;
	int i;
	for(i=2;i<sqrt(x);i++)
	{
		if(x%i==0){
		ret=0;
		break;}	
	}
	return ret;
}
