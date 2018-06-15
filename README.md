# calculator1
进行简单的加、减、乘、除、开方等运算
#include<stdio.h>
#include<math.h>
using namespace std;

double Plus(double number1,double number2)
{

    double temp;
    temp = number1+number2;
    return temp;
}

int main()
{

    double  number1,number2;
    int key;

    printf("选择运算法则：1:加法\n2:减法\n3:乘法\n4:开根号\n5:除法");
    scanf("%d",&key);
    switch(key)
    {

    case 1:

        printf("请输入要计算的两位数");


        scanf("%d %d",&number1,&number2);

        printf(Plus(number1,number2));
        break;
    case 2:

        printf("请输入要计算的两位数");


        scanf("%d %d",&number1,&number2);

        printf(subtraction(number1,number2));
        break;
    case 3:

        printf("请输入要计算的两位数");


        scanf("%d %d",&number1,&number2);

        printf(multiplication(number1,number2));
        break;
    case 4:

        printf("请输入要计算的数");

        scanf("%d",&number1);

        printf(sqrt(number1));
        break;
    case 5:

        printf("请输入要计算的两位数");


        scanf("%d %d",&number1,&number2);

        printf(division(number1,number2));
        break;

    }
    return 0;
}
