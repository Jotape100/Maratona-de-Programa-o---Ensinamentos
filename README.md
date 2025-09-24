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
--------------------------------------------------------------------------------------------------------------------------------------------


    
    return 0;
}
