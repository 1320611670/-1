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





#define _CRT_SECURE_NO_WARNINGS 
#include <iostream>

int main()
{
	//int a = 0;
	//int b = 2;
	//if (a == 1)
	//{
	//	if (b == 2)
	//		printf("hehe\n");
	//}
	//	else
	//		printf("haha\n");
	//return 0;
	/*return 0;
	int i=1;
	while(i<=100)
	{
		if (i % 2 == 1)
			printf("%d ", i);
		i++;
	}*/
	/*int day = 0;
	scanf("%d", &day);
	switch (day)
	{
	case 1:
		printf("星期一\n");
		break;
	case 2:
		printf("星期二\n");
		break;
	case 3:
		printf("星期三\n");
		break;
	case 4:
		printf("星期四\n");
		break;
	case 5:
		printf("星期五\n");
		break;
	case 6:
		printf("星期六\n");
		break;
	case 7:
		printf("星期日\n");
		break;
	default:
		printf("输入错误\n");
		break;
	}
	return 0;*/
	/*int n = 1;
	int m = 2;
	switch (n)
	{
	case 1:m++;
	case 2:n++;
	case 3:
		switch (n)
		{
		case 1:n++;
		case 2:m++; n++; break;
		}
	case 4:m++;
		break;
	default:
		break;
	}
	printf("m=%d,n=%d\n", m, n);
	return 0;*/
	/*int ch = 0;
	while ((ch = getchar()) != EOF)
	{
		putchar(ch);
	}
	return 0;*/
	//int ch = 0;
	//int ret = 0;
	//char password[20] = { 0 };
	//printf("请输入密码:");
	//scanf("%s", password);
	//while (ch = getchar() != '\n')
	//{
	//	;
	//}
	//printf("请确认Y/N");
	//ret = getchar();
	//if (ret == 'Y')
	//	printf("确认成功\n");
	//else
	//	printf("确认失败\n");
	//return 0;
	int ch = 0;
	while ((ch = getchar()) != EOF)
	{
		if (ch<'0' || ch>'9')
			continue;
		putchar(ch);
	}
	return 0;
}

