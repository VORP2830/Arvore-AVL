# Árvore AVL

Esta é uma implementação de Árvore AVL (Adelson-Velskii e Landis) em Python. A árvore AVL é uma árvore de busca binária auto balanceada que mantém uma árvore equilibrada realizando rotações. A árvore é equilibrada garantindo que as alturas das subárvores esquerda e direita diferem no máximo uma unidade. A classe `Arvore` implementa a estrutura de dados Árvore AVL, e a classe `No` implementa o nó individual da árvore AVL.

## Classe No

A classe `No` representa um nó individual da árvore AVL.

### Propriedades

- `valor`: um valor inteiro que representa o valor do nó.
- `esquerda`: uma referência ao filho esquerdo do nó.
- `direita`: uma referência ao filho direito do nó.
- `Altura`: um valor inteiro que representa a altura do nó.

## Classe Arvore

A classe `Arvore` representa a estrutura de dados Árvore AVL.

### Métodos

- `Altura(self, no)`: um método auxiliar para obter a altura de um nó na árvore AVL.

  - `no`: uma referência ao nó cuja altura deve ser encontrada.
  - Retorna um valor inteiro representando a altura do nó fornecido.

- `Balanceado(self, no)`: um método auxiliar para obter o fator de equilíbrio de um nó na árvore AVL.

  - `no`: uma referência ao nó cujo fator de equilíbrio deve ser encontrado.
  - Retorna um valor inteiro representando o fator de equilíbrio do nó fornecido.

- `RotacaoDireita(self, no)`: um método auxiliar para realizar uma rotação à direita em um nó na árvore AVL.

  - `no`: uma referência ao nó a ser rotacionado.
  - Retorna uma referência à nova raiz da subárvore após a rotação.

- `RotacaoEsquerda(self, no)`: um método auxiliar para realizar uma rotação à esquerda em um nó na árvore AVL.

  - `no`: uma referência ao nó a ser rotacionado.
  - Retorna uma referência à nova raiz da subárvore após a rotação.

- `Inserir(self, val, raiz)`: um método para inserir um novo nó com um valor fornecido na árvore AVL.

  - `val`: um valor inteiro representando o valor do novo nó a ser inserido.
  - `raiz`: uma referência à raiz da subárvore na qual o novo nó deve ser inserido.
  - Retorna uma referência à nova raiz da subárvore após a inserção.

- `InOrder(self, raiz)`: um método para percorrer a árvore AVL em Ordem (Esquerda-Raiz-Direita) e imprimir o valor de cada nó.

  - `raiz`: uma referência à raiz da subárvore a ser
