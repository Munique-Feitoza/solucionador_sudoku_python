# 🧩 Sudoku Solver em Python

Este projeto é um **resolvedor de Sudoku** implementado em Python. Ele recebe um tabuleiro incompleto como entrada e utiliza **backtracking** para encontrar uma solução válida para o quebra-cabeça.

---

## 🔍 Funcionalidades

- Resolve quebra-cabeças Sudoku 9x9 utilizando **algoritmo de backtracking**.
- Valida tentativas com base nas **regras do Sudoku**:
  - O número deve ser único na linha.
  - O número deve ser único na coluna.
  - O número deve ser único na subgrade 3x3.
- Exibe o quebra-cabeça antes e depois da resolução.

---

## 🛠️ Estrutura do Código

### `Board` (classe principal)
Responsável por:
- Armazenar o tabuleiro.
- Imprimir o tabuleiro.
- Verificar células vazias.
- Verificar se um número é válido na linha, coluna e subgrade.
- Executar a resolução do Sudoku com **backtracking recursivo**.

### `solve_sudoku(board)`
Função utilitária que:
- Cria uma instância de `Board`.
- Exibe o quebra-cabeça.
- Resolve e exibe a solução (se existir).

---

## ▶️ Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/sudoku-solver.git
   cd sudoku-solver
   ```

2. Execute o script Python:
   ```bash
   python sudoku_solver.py
   ```

---

## 🧪 Exemplo de Entrada

```python
puzzle = [
  [0, 0, 2, 0, 0, 8, 0, 0, 0],
  [0, 0, 0, 0, 0, 3, 7, 6, 2],
  [4, 3, 0, 0, 0, 0, 8, 0, 0],
  [0, 5, 0, 0, 3, 0, 0, 9, 0],
  [0, 4, 0, 0, 0, 0, 0, 2, 6],
  [0, 0, 0, 4, 6, 7, 0, 0, 0],
  [0, 8, 6, 7, 0, 4, 0, 0, 0],
  [0, 0, 0, 5, 1, 9, 0, 0, 8],
  [1, 7, 0, 0, 0, 6, 0, 0, 5]
]
```

---

## ✅ Saída Esperada

```
Puzzle to solve:
* * 2 * * 8 * * *
* * * * * 3 7 6 2
4 3 * * * * 8 * *
...

Solved puzzle:
7 1 2 6 9 8 5 3 4
3 9 8 1 5 3 7 6 2
4 3 6 2 7 0 8 1 9
...
```

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

