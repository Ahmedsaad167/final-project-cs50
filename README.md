# Equation Assistant

Equation Assistant the progrem works in the work of mathematical and accounting equations with this program only

## Project Sections
- Math

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
}

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
![1](https://raw.githubusercontent.com/Ahmedsaad167/final-project-cs50/main/1.png)
<br>
![2](https://raw.githubusercontent.com/Ahmedsaad167/final-project-cs50/main/2.png)
<br>
![1](https://raw.githubusercontent.com/Ahmedsaad167/final-project-cs50/main/3.png)
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
![1](https://raw.githubusercontent.com/Ahmedsaad167/final-project-cs50/main/4.png)
<br>
![1](https://raw.githubusercontent.com/Ahmedsaad167/final-project-cs50/main/5.png)
<br>
<hr>

## Library
- stdio.h
- cs50.h
- stdlib.h
