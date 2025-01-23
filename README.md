# Calculator
# work -->This program allows the user to input two numbers and an operator, and it performs the corresponding calculation based on the operator.
#include <stdio.h>

int main()
{
    double num1, num2, result;
    char operator;
    printf("Enter the 1st number :");
    scanf("%lf", &num1);
    printf("Enter the 2nd number :");
    scanf("%lf", &num2);

    printf(" Enter the operator (+,-,*,/) :");
    scanf("%s", &operator);
    switch (operator)
    {
    case '+':
        result = num1 + num2;
        printf("%lf", result);
        break;
    case '-':
        result = num1 - num2;
        printf("%lf", result);
        break;
    case '*':
        result = num1 * num2;
        printf("%lf", result);
        break;
    case '/':
        if (num2 != 0)
        {
            result = num1 / num2;
            printf("%lf", result);
            break;
        }
        else
        {
            printf(" this is not valid num2 cant be zero:");
            break;
        }

    default:
        printf(" operator is invalid pls select the given operator(+,-,*,/) :");
        break;
    }
    return 0;
}
