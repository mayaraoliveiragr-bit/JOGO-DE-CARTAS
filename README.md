# JOGO-DE-CARTAS

#include <stdio.h>

int main (){

//DADOS CARTA 1
 char estado1 []="RJ"; // Uma letra de 'A' a 'H' (representando um dos oito estados). Tipo: char
 char codigo1 [20]; //A letra do estado seguida de um número de 01 a 04 
 char cidade1 [20] = "RIO DE JANEIRO"; //O nome da cidade.
 int populacao1 = 55600; //O número de habitantes da cidade
 float area1 = 200.000;//A área da cidade em quilômetros quadrados.
 float pib1 = 5.6;//O Produto Interno Bruto da cidade.
 int turistico1; //A quantidade de pontos turísticos na cidade.

 //DADOS CARTA 2
 char estado2 []= "SP"; // Uma letra de 'A' a 'H' (representando um dos oito estados). Tipo: char
 char codigo2 [20]; //A letra do estado seguida de um número de 01 a 04 
 char cidade2 [20] = "SÃO PAULO"; //O nome da cidade.
 int populacao2 = 60600; //O número de habitantes da cidade
 float area2 = 100.000;//A área da cidade em quilômetros quadrados.
 float pib2 = 5.5;//O Produto Interno Bruto da cidade.
 int turistico2; //A quantidade de pontos turísticos na cidade.


//ATRIBUTO: DENSIDADE POPULACIONAL
 printf("CARTA 1\n");
 float DensidadePopulacional = populacao1/area1;
 printf ("Densidade Populacional %s: %f\n", estado1, DensidadePopulacional);

 float PibPerCapita = pib1/populacao1;
 printf ("PIB per capita %s: %f\n", estado1, PibPerCapita);

 printf("CARTA 2\n");
 float DensidadePopulacional1 = populacao2/area2;
 printf ("Densidade Populacional %s: %f\n", estado2, DensidadePopulacional1);

 float PibPerCapita1 = pib2/populacao2;
 printf ("PIB per capita %s: %f\n", estado2, PibPerCapita1);

 if ( DensidadePopulacional < DensidadePopulacional1){
    printf("Resultado: Carta 2 - %s, venceu!\n", cidade2);
 } else {
    printf("Resultado: Carta 1 - %s, venceu!\n", cidade1);
 }
 return 0;
}
