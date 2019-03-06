# Exercicio23

#include <stdlib.h>
#include <stdio.h>
#include <string.h>

int main() {

int i;
char pala1[20],pala2[20];
char *ptr, *ptr1;

printf("Digite uma palavra ");
gets(pala1);

printf("Digite outra ");
gets(pala2);

ptr=strstr(pala1,pala2);

for (i=0; i<=19; i++)
{
    if (pala1[i]==ptr)
    {ptr1=&pala1[i];}
}
printf("endereco %x\n", ptr1);
return 0;
}
