Este projeto é uma simulação do jogo Batalha Naval, implementado na linguagem C, utilizando vetores unidimensionais para representar um tabuleiro de 10x10.

1. O código posiciona dois navios de tamanho 3 no tabuleiro:
- Um navio posicionado horizontalmente.
- Um navio posicionado verticalmente.

2. O programa realiza a validação de:
- Limites do tabuleiro (para garantir que o navio não fique fora da grade).
- Sobreposição (os navios não podem ocupar as mesmas células).

3. Após o posicionamento, o programa exibe o tabuleiro no console, onde:
- 0 representa água.
- 3 representa as partes dos navios.

Como Funciona:
O tabuleiro é representado por um vetor de tamanho 100, onde cada célula do tabuleiro é acessada através da fórmula:
índice = linha * 10 + coluna

Exemplo: Para acessar a célula da linha 2, coluna 3:
índice = 2 * 10 + 3 = 23

Exemplo de Saída:

    0  1  2  3  4  5  6  7  8  9 
 0  0  0  0  0  0  0  0  0  0  0 
 1  0  0  0  0  0  0  0  0  0  0 
 2  0  0  0  3  3  3  0  0  0  0 
 3  0  0  0  0  0  0  0  0  0  0 
 4  0  0  0  0  0  0  0  0  0  0 
 5  0  0  0  0  0  0  0  3  0  0 
 6  0  0  0  0  0  0  0  3  0  0 
 7  0  0  0  0  0  0  0  3  0  0 
 8  0  0  0  0  0  0  0  0  0  0 
 9  0  0  0  0  0  0  0  0  0  0 


Estrutura do Código:
- inicializarTabuleiro: Preenche o vetor com 0 (água).

- posicionarNavio: Posiciona um navio no tabuleiro na orientação desejada (H para horizontal e V para vertical), realizando validações.

- exibirTabuleiro: Mostra o tabuleiro no console com linhas e colunas identificadas.

- main: Define as coordenadas dos dois navios, executa as funções de posicionamento e imprime o tabuleiro.
