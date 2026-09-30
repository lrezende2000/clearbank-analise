# ClearBank — Análise Financeira de Transações

Projeto do desafio final do módulo de Análise de Dados (pós-graduação em IA e Automações).
O notebook lê `transacoes.csv`, valida e limpa os registros, calcula métricas financeiras
mensais, sinaliza transações suspeitas (acima de R$ 10.000) e exporta `relatorio.json`.

## Como executar
1. Abra o `desafio-final.ipynb` no Google Colab ou Jupyter.
2. Execute todas as células em ordem (a Célula 0 cria o `transacoes.csv` de teste).
3. A Célula de Execução Principal gera o relatório no terminal e o `relatorio.json`.

## Saídas geradas
- Relatório formatado no terminal (resumo mensal, período e suspeitas).
- `relatorio.json` com totais, resumo mensal e transações suspeitas.
- `grafico.png` (opcional — saldo mensal por mês).

## Estrutura
- `desafio-final.ipynb` — notebook com código e saídas salvas
- `grafico.png` — gráfico matplotlib (opcional)
