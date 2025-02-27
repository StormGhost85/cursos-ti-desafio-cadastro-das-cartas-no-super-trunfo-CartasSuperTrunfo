#include <stdio.h>
#include <string.h>

// Definindo o tamanho máximo para strings
#define MAX_STRING 100

// Estrutura para representar uma carta do Super Trunfo
typedef struct {
    char estado;
    char codigo[4]; // 3 caracteres + '\0'
    char nome_cidade[MAX_STRING];
    int populacao;
    float area;
    float pib;
    int pontos_turisticos;
} Carta;

// Função para ler os dados de uma carta
void lerCarta(Carta *carta, int numero_carta) {
    printf("\nInsira os dados da Carta %d:\n", numero_carta);
    printf("Estado (A-H): ");
    scanf(" %c", &carta->estado);

    printf("Código da Carta (ex: A01): ");
    scanf("%s", carta->codigo);

    printf("Nome da Cidade: ");
    scanf(" %[^\n]", carta->nome_cidade); // Lê até encontrar uma nova linha

    printf("População: ");
    scanf("%d", &carta->populacao);

    printf("Área (em km²): ");
    scanf("%f", &carta->area);

    printf("PIB (em bilhões de reais): ");
    scanf("%f", &carta->pib);

    printf("Número de Pontos Turísticos: ");
    scanf("%d", &carta->pontos_turisticos);
}

// Função para exibir os dados de uma carta de forma organizada
void exibirCarta(Carta carta, int numero_carta) {
    printf("\nCarta %d:\n", numero_carta);
    printf("Estado: %c\n", carta.estado);
    printf("Código: %s\n", carta.codigo);
    printf("Nome da Cidade: %s\n", carta.nome_cidade);
    printf("População: %d\n", carta.populacao);
    printf("Área: %.2f km²\n", carta.area);
    printf("PIB: %.2f bilhões de reais\n", carta.pib);
    printf("Número de Pontos Turísticos: %d\n", carta.pontos_turisticos);
}

int main() {
    Carta carta1, carta2;

    // Ler os dados das duas cartas
    lerCarta(&carta1, 1);
    lerCarta(&carta2, 2);

    // Exibir os dados das duas cartas de forma organizada
    exibirCarta(carta1, 1);
    exibirCarta(carta2, 2);

    return 0;
}

