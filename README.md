# Maratona-de-Programa-o---Ensinamentos
Todos os Códigos sobre maratona que eu achar relevante lembrar, além de funções também

CODIGO DE VETOR DE FREQUENCIA

#include <bits/stdc++.h>

using namespace std;

int main()
{
    //Criei um vetor de posicoes e os numeros que iria digitar
    int N, vet[2001], numeros;

    //Zerei o Vetor para tirar lixo de memoria
    for(int i = 0; i < 2001; i++)
    {
        vet[i] = 0;
    }

    //Li os numeros de testes
    scanf("%d", &N);
    for(int i = 0 ; i< N; i++)
    {
        //li os numeros e acrescentei cada vez o numero de POSICAO desse vetor
        scanf("%d", &numeros);
        vet[numeros]++;

    }
    //Printei se aquele vetor foi acrescentado
    for(int k = 0; k < 2001; k++)
    {
        for(int z = 0; z < vet[k]; z++)
        {
            if(vet[k] > 0)
            {
                printf("%d aparece %d vez(es)\n", k, vet[k]);
                break;
            }
        }
    }

    CODIGO DE MMC COM MDC DE FRAÇÕES
    #include <bits/stdc++.h>

using namespace std;

int MDC(int a, int b)
{
    while(b != 0)
    {
        int resto = a % b;
        a = b;
        b = resto;
    }
    return a; 
}

int main()
{
   char sinal;
   char barra = '/';
   int conta;

   int N1,N2,D1,D2;
   int N;

   int resultado,Ds;
   int Mdc;

   scanf("%d", &N);
   getchar();

   for(int i = 0; i < N; i++)
   {
    scanf("%d %c %d %c %d %c %d", &N1, &barra, &D1, &sinal, &N2, &barra, &D2);
    getchar();

    Ds = D1 * D2;
   if(sinal == '+')
   {
    conta = (N1*D2 + N2*D1);
    resultado = Ds;
    
   }
   else if(sinal == '-') 
   {
   conta = (N1*D2 - N2*D1);
   resultado = Ds;

   }
   else if(sinal == '/')
   {
    conta = (N1*D2);
    resultado = (N2 * D1);
   }
   else if(sinal == '*') 
   {
     conta = (N1*N2);
     resultado = Ds;
   }

   Mdc = MDC(abs(conta),abs(resultado));
   printf("%d/%d = %d/%d\n",conta,resultado, conta/Mdc, resultado/Mdc);

   }

    return 0;
}
--------------------------------------------------------------------------------------------------------------------------------------------


    
    return 0;
}
