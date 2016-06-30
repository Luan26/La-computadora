# La-computadora
A very simple calculator of BMI

#include <stdio.h>
#include <conio.h>
#include <math.h>
#define LIMITE 30 // Constante local 

int main() {
	
float peso, altura, imc;

int clrscr(); // Esta função limpa a tela

printf("\n Qual o seu peso e altura? ");

scanf("%f, %f", &peso, &altura);

imc = peso/pow(altura,2);// pow é uma função matemática para Expoente

printf("\n Seu i.m.c. eh %.1f \n", imc);

if( imc <= LIMITE ) 
{
printf("\n Voce nao esta obeso! \n");
}

else
{
 printf("\n Voce esta obeso! \n");
}

getch(); //Esta função fecha o programa ao pressionar qualquer tecla 

}
