# README — Bruna Leal — T3

## O que eu estou entregando

- `Miniprojeto_Varejo.ipynb` — meu notebook com a Análise Exploratória de Dados (AED) da
  base Varejo.
- `df_limpo.csv` — a base depois de eu limpar (gerada pelo próprio notebook).
- `Base Varejo.csv` — a base original que eu usei como ponto de partida (baixei do Kaggle).

## Como eu rodo isso (ou como você pode rodar também)

### Opção 1 — Google Colab
1. Entro no [Google Colab](https://colab.research.google.com/) e faço upload do arquivo
   `miniprojeto_Bruna.ipynb`.
2. Faço upload também do `Base Varejo.csv` pro ambiente do Colab (ou monto o Google Drive
   e ajusto o caminho do arquivo na primeira célula).
3. Rodo todas as células, em ordem (`Ambiente de execução > Executar tudo`).

### Opção 2 — VS Code
1. Instalo as extensões **Python** e **Jupyter** no VS Code.
2. Abro a pasta do projeto e o arquivo `miniprojeto_Bruna.ipynb`.
3. Confiro se o `Base Varejo.csv` está na mesma pasta do notebook.
4. Instalo o pandas, se ainda não tiver:
   ```
   pip install pandas
   ```
5. Rodo todas as células do notebook, em ordem.

## O que esperar quando rodar

No final da execução, o notebook mostra o diagnóstico de qualidade dos dados, as
estatísticas da coluna de número de filhos do cliente, os agrupamentos que eu fiz e o bloco
de conclusões — e também gera o arquivo `df_limpo.csv` com a base já tratada.
