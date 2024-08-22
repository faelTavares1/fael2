1) Qual biblioteca é necessaria incluir com diretiva #include para usar as funçoes de entrada pasrao de linguagem c?

R:Para usar as funções de entrada e saída padrão em C, você deve incluir a biblioteca <stdio.h>. Ela define funções como printf e scanf.
#include <stdio.h>


2) O trecho de codigo realiza a lei de um numero inteiro entretanto,ele contém dois erros. Corrija-os e justifique sua resposta
   Int n;
   Scanf ("%f", n);
   
   R:Erro 1: O tipo de dado especificado no scanf não corresponde ao tipo da variável. Para ler um inteiro, você deve usar %d em vez de %f, que é usado para números de ponto flutuante.
   Erro 2: A função scanf deve passar a variável por referência, usando o operador &. Além disso, a palavra-chave deve ser int (com "i" minúsculo) e scanf deve ser em minúsculas.

Código corrigido:
int n;
scanf("%d", &n);

3) Explique o trecho de código abaixo (linha 2)
   
   char c;
   scanf ("%c",& C);
   While (getchar C) != '\n');
   scanf("%c", &c);

R:Lê um caractere da entrada padrão e armazena na variável c.
while (getchar() != '\n');: Este loop lê caracteres da entrada padrão até encontrar um caractere de nova linha (\n). Isso é usado para consumir qualquer entrada restante na linha após o caractere lido por scanf. Isso é útil para limpar o buffer de entrada, especialmente quando se alterna entre diferentes tipos de entrada (por exemplo, de números para caracteres).
   

4) Explique o trecho de código abaixo 
 
   Float largura, comprimento ,
   scanf ("%F%F, &larguera, &comprimento);

R:float largura, comprimento;: Declara duas variáveis do tipo float, que armazenarão números de ponto flutuante.

scanf("%f %f", &largura, &comprimento);: Lê dois números de ponto flutuante da entrada padrão e armazena-os nas variáveis largura e comprimento, respectivamente. O formato %f é usado para números de ponto flutuante.
5) Explique o trecho de codigo abaixo 

   char nome [80];
   scanf ("%s",nome);
  
   R:char nome[80];:Declara um array de caracteres com tamanho 80, que pode armazenar uma string de até 79 caracteres mais o terminador nulo (\0).
scanf("%s", nome);: Lê uma string da entrada padrão e a armazena no array nome. O formato %s é usado para strings, e scanf automaticamente adiciona o terminador nulo (\0) ao final da string.

6) Explique o trecho de codigo abaixo 

   paintf ("ola, mundo!"),

    R:printf("ola, mundo!");: Esta linha de código imprime a string "ola, mundo!" na saída padrão (normalmente o console). A função printf é usada para saída formatada em C e pode incluir variáveis e formatar a saída conforme especificado pelos seus parâmetros.
