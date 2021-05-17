#include<stdio.h>
#include<cs50.h>
int main()
{
string name;
float m,BMI;
int kg;
name=get_string("Enter the name ");
m=get_float("Enter your height (in m) ");
kg=get_int("Enter your weight (in kg) ");
BMI=(float)(kg/(m*m));
if(BMI<18.5)
{
printf("%s %.2f underweight\n",name,BMI);
}
else if(BMI>=18.5 && BMI<=24.9)
{
printf("%s %.2f normal weight\n",name,BMI);
}
else if(BMI>=25 && BMI<=29.9)
{
printf("%s %.2f overweight\n",name,BMI);
}
else
{
printf("%s %.2f obese\n",name,BMI);
}
return 0;
}
