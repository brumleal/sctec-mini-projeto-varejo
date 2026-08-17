# Mini-Projeto Avaliativo — Análise Exploratória de Dados (Base Varejo)

## Sobre o projeto

Esse é o meu mini-projeto da disciplina de BI e Visualização de Dados. Nele eu fiz uma
Análise Exploratória de Dados (AED) usando a base **Varejo**, que tem registros de compras
(data, cliente, produto e categoria).

O objetivo foi praticar o passo a passo de uma AED: carregar os dados, verificar problemas
de qualidade, limpar a base, calcular estatísticas descritivas e explorar alguns padrões
por meio de agrupamentos, terminando com um resumo dos principais insights que encontrei.

## O que tem neste repositório

- `miniprojeto_Bruna.ipynb` — meu notebook com todo o código comentado, dividido nas
  etapas pedidas: carga dos dados, diagnóstico, limpeza, estatística descritiva,
  agrupamentos e conclusões.
- `df_limpo.csv` — a base já tratada, gerada no final do notebook (separador `;`).
- `Readme_BrunaLeal_T3.md` — instruções de como rodar o meu projeto.

## De onde vieram os dados

Usei a base "Varejo" disponível no Kaggle:
https://www.kaggle.com/datasets/namespaiva/base-varejo/data

## O que eu fiz, resumindo

1. **Carreguei os dados:** li o `Base Varejo.csv` (separador `;`) e removi umas colunas
   vazias que vieram junto por causa de um problema no arquivo original.
2. **Verifiquei a qualidade:** contei valores nulos, encontrei que cerca de 11,6% das
   linhas eram duplicadas e que ~0,44% dos registros tinham a categoria do produto marcada
   como `#N/D` (ou seja, sem categoria).
3. **Limpei a base:**
   - Tirei as linhas com categoria `#N/D`, porque eram bem poucas e eu não quis "inventar"
     uma categoria pra elas.
   - Removi as linhas totalmente duplicadas.
   - Converti a coluna `DATA` pra formato de data de verdade (`datetime`) e as colunas
     categóricas (`CL_GENERO`, `CL_SEG`, `PR_CAT`) para o tipo `category`.
4. **Calculei estatísticas** da coluna `CL_FHL` (número de filhos do cliente): média,
   mediana, desvio padrão, moda, máximo, mínimo e contagem.
5. **Explorei alguns agrupamentos:** total de itens comprados por gênero, total vendido por
   categoria de produto, e como as vendas variam mês a mês.
6. **Escrevi minhas conclusões** com os principais insights que encontrei e o que ainda
   ficou faltando resolver na base.

## O que usei

- Google Colab / Notebook
- Python 3
- pandas

## Como rodar

Isso está explicado com mais detalhe no arquivo `Readme_BrunaLeal_T3.md`.
