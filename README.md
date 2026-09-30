# ClearBank — Análise Financeira de Transações

Projeto do desafio final do módulo de Análise de Dados (pós-graduação em IA e Automações).
O notebook lê `transacoes.csv`, valida e limpa os registros, calcula métricas financeiras
mensais, sinaliza transações suspeitas (acima de R$ 10.000) e exporta `relatorio.json`.

## Como executar

1. Abra o `desafio-final.ipynb` no Google Colab ou Jupyter.
2. Execute todas as células em ordem (a Célula 0 cria o `transacoes.csv` de teste).
3. A Célula de Execução Principal gera o relatório no terminal e o `relatorio.json`.

## Requisito Opcional RO1 — Análise com pandas

Este projeto também implementa o requisito opcional de análise com pandas.
A versão alternativa está em um arquivo separado, `analise_pandas.py`, para não
misturar com a solução principal (que usa apenas módulos nativos do Python).

O script carrega o `transacoes.csv` com `pd.read_csv()`, aplica as mesmas regras de
validação da solução nativa, agrupa as métricas por mês com `groupby`/`pivot_table`
e compara os resultados com o `relatorio.json` — os valores devem ser idênticos.

### Como executar a versão com pandas

- **No Google Colab:** faça o upload do `analise_pandas.py` (ou cole o conteúdo em
  uma célula do notebook), garanta que o `transacoes.csv` já foi gerado pela Célula 0
  e execute. O pandas já vem instalado no Colab.
- **Localmente:** com Python 3.10+ instalado, rode:

  ```bash
  pip install pandas
  python analise_pandas.py
