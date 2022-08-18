# Equation Assistant

Equation Assistant the progrem works in the work of mathematical and accounting equations with this program only

### Project Demo

https://youtu.be/lqGGeCd5R0s

## Project Sections
- Math

`
int math()
{
    int service =
        get_int("\nChoose the equation\n\n1- Summation(+)\n2- Minus(-)\n3- Multiply(X)\n4- Division(/)\n5- Average \n Number: ");
    float num1 = get_float("Number1: ");
    float num2 = get_float("Number2: ");
    if (service == 1)
    {
        sum(num1, num2);
    }
    else if (service == 2)
    {
        minus(num1, num2);
    }
    else if (service == 3)
    {
        multiply(num1, num2);
    }
    else if (service == 4)
    {
        division(num1, num2);
    }
    else if (service == 5)
    {
        avg(num1, num2);
    }
    return 0;
}`

- Accounting

`
int acounting()
{
    int acc = get_int("\nChoose the equation\n\n1- Vat (.14)\n2- Residual(.01)\n3- Both\nNumber: ");
    float total = get_float("\nTotal: ");
    float tax = total * .14;
    float dud = total * .01;
    float both = total + tax - dud;
}`

### Math Sections
- sum : to collect numbers.

`
int sum(float num1, float num2)
{
    printf("\nSum: %.2f\n", num1 + num2);
    return 0;
}
`
- minus : to subtract numbers.
`int minus(float num1, float num2)
{
    printf("\nMinus: %.2f\n", num1 - num2);
    return 0;
}

`

- multiply : to multiply numbers.

`
int multiply(float num1, float num2)
{
    printf("\nMultiply: %.2f\n", num1 * num2);
    return 0;
}`
- division : Divide numbers by one.

`
int division(float num1, float num2)
{
    printf("\nDivision: %.2f\n", num1 / num2);
    return 0;
}`
- average : Calculate the average between two numbers.

`
int avg(float num1, float num2)
{
    printf("\nAverage: %.2f\n", (num1 + num2) / 2);
    return 0;
}`
<hr>
![1](https://user-images.githubusercontent.com/108421177/185293267-d75fb1a4-7a19-4afc-92fc-5e0f018815f8.png)
![2](https://user-images.githubusercontent.com/108421177/185293270-a1af9d95-dd4d-447a-8c61-8db5d6b07a63.png)
![3](https://user-images.githubusercontent.com/108421177/185293273-bd10a4a0-eae9-4828-b112-dd1deebeb219.png)
<br>

### Accounting Sections
- Vat : It is 14% of the net product and added to the net and paid by the final consumer

`
if (acc == 1)
    {
        printf("Tax: %.2f\n", tax);
        printf("Net: %.2f\n", total + tax);
    }`
- Duduction : 1% of the net product will be deducted from the net

`
    else if (acc == 2)
    {
        printf("Deduction: %.2f\n", dud);
        printf("Net: %.2f\n", total - dud);
    }`
- Both : VAT is added to the net, then 1% of the net is deducted from the total product

`
   else if (acc == 3)
    {
        printf("Tax: %.2f\n", tax);
        printf("Duducation: %.2f\n", dud);
        printf("Net: %.2f\n", both);
    }`
<hr>
![4](https://user-images.githubusercontent.com/108421177/185293274-b18be313-277b-4583-913b-649735b53ae1.png)
<br>
![5](https://user-images.githubusercontent.com/108421177/185293263-8478ad0c-2f7d-4a4f-85bd-c286c05bf161.png)
<br>
<hr>

## Library
- stdio.h
- cs50.h
- stdlib.h
