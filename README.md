#define  _CRT_SECURE_NO_WARNINGS  1

#include <iostream>

//int main()
//{
//	/*
//	int num1 = 0;
//	int num2 = 0;
//	int sum = 0;
//	scanf("%d%d", &num1,&num2);
//	sum = num1 + num2;
//	printf("sum=%d\n", sum);
//	*/
//	/*char arr1[] = "abc";
//	char arr2[] = { 'a','b','c','\0' };
//	printf("%s\n", arr1);
//	printf("%s\n", arr2);
//	return 0;*/
//	//int input = 0;
//	//printf("加入天启\n");
//	//printf("你要改变世界吗？（1/0）>:");
//	//scanf("%d", &input);
//	//if (input == 1)
//	//	printf("改变世界\n");
//	//else
//	//	printf("被世界改变\n");
//	//return 0;
//}#include <iostream>

int Max(int x, int y)
{
	if (x > y)
		return x;
	else
		return y;
}

int main()
{
	/*int num1 = 10;
	int num2 = 20;
	if (num1 > num2)
		printf("较大值是%d\n", num1);
	else
		printf("较大值是%d\n", num2);
	return 0;*/

	int num1 = 10;
	int num2 = 20;
	int max = 0;
	max = Max(num1, num2);
	printf("max=%d\n", max);
	return 0;

}

