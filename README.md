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

#define _CRT_SECURE_NO_WARNINGS
#include <iostream>
#include<windows.h>

int main()
{
	/*int i = 1;
	do
	{
		printf("%d", i);
		i++;
	}
	while (i <= 10);
		return 0;*/
		/*int i=0;
		int n = 0;
		int ret = 0;
		for (n = 1; n <= 3; n++)
		{
			int sum = 1;
			for (i = 1; i <= n; i++)
			{
				sum = sum * i;
			}
			ret = ret + sum;
		}
		printf("%d\n", ret);
		return 0;*/

		//简化版本
		/*int n=0;
		int ret = 1;
		int sum = 0;
		for (n = 1; n <= 3; n++)
		{
			ret = ret * n;
			sum = ret + sum;
		}
		printf("sum=%d\n", sum);
		return 0;*/
		/*int arr[] = { 1,2,3,4,5,6,7,8,9,10 };
		int k =17;
		int i = 0;
		int sz = sizeof(arr) / sizeof(arr[0]);
		for (i = 0; i < sz; i++)
		{
			if (k == arr[i])
			{
				printf("下标是%d\n", i);
				break;
			}
		}
		if (i == sz)
			printf("找不到\n");
		return 0;*/

	/*char arr1[] = "welcome to bit!!!!!" ;
	char arr2[] =  "###################" ;
	int left = 0;
	int right = strlen(arr1) - 1;
	while (left <= right)
	{
		arr2[left] = arr1[left];
		arr2[right] = arr1[right];
		printf("%s\n", arr2);
		Sleep(1000);
		left++;
		right--;
	}
	return 0;*/

	int i = 0;
	char password[20] = { 0 };
	for (i = 0; i < 3; i++)
	{
		printf("请输入密码：");
		scanf("%s", password);
		if (strcmp(password, "123456") == 0)
		{
			printf("登录成功\n");
			break;
		}
		else
		{
			printf("密码错误\n");
		}
	}
	if (i == 3)
		printf("密码三次错误10分钟后重试\n");
	return 0;

}

#define _CRT_SECURE_NO_WARNINGS 
#include <iostream>

int binary_search(int arr[], int k, int sz)
{
	int left = 0;
	int right = sz - 1;
	while (left <= right)
	{
		int mid = (left + right) / 2;
		if (arr[mid] < k)
		{
			left = mid + 1;
		}
		else if (arr[mid] > k)
		{
			right = mid - 1;
		}
		else
		{
			return mid;
		}
	}
	return -1;
}

void print(int n)
{
	if (n > 9)
	{
		print(n / 10);
	}
	printf("%d ", n % 10);
}

int my_strlen(char*str)
{
	if (*str != '\0')
		return 1 + my_strlen(str + 1);
	else
		return 0;
}

int Fac(int n)
{
	if (n <= 1)
		return 1;
	else
		return n * Fac(n - 1);
}

//int Fib(int n)
//{
//	if (n <= 2)
//		return 1;
//	else
//		return Fib(n - 1) + Fib(n - 2);
//}

int Fib(int n)
{
	int a = 1;
	int b = 1;
	int c = 1;

	while (n > 2)
	{
		c = a + b;
		a = b;
		b = c;
		n--;
	}
	return c;
}

int main()
{
	//int arr[] = { 1,2,3,4,5,6,7,8,9,10 };
	//int k = 2;
	//int sz = sizeof(arr) / sizeof(arr[0]);
	//int ret = binary_search(arr, k, sz);
	//if (ret == -1)
	//{
	//	printf("找不到指定数字\n");
	//}
	//else
	//{
	//	printf("找到了，下标是：%d\n", ret);
	//}
	//return 0;

	//unsigned int num = 0;
	//scanf("%d", &num);
	//print(num);
	//return 0;
/*
	char arr[] = "bit";
	int len = my_strlen(arr);
	printf("len=%d\n", len);
	return 0;*/

	/*int n = 0;
	int ret = 0;
	scanf("%d", &n);
	ret = Fac(n);
	printf("%d\n", ret);
	return 0;*/

	int n = 0;
	int ret = 0;
	scanf("%d", &n);
	ret = Fib(n);
	printf("%d\n", ret);
	return 0;

}

