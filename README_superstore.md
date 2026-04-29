# Análise Financeira Empresarial — Superstore

Análise exploratória de dados de vendas de uma rede de lojas americana, com foco em lucratividade, desempenho por categoria, comportamento de descontos e análise regional.

---

## Sobre o Dataset

| Info | Valor |
|---|---|
| Fonte | Kaggle — Superstore Sales Dataset |
| Total de registros | 9.994 pedidos |
| Período | 2014 a 2017 |
| Variáveis | Vendas, Lucro, Desconto, Categoria, Subcategoria, Segmento, Região, Estado, Clientes |

---

## Análises Realizadas

### Vendas e Receita
- Faturamento total por ano
- Sazonalidade — faturamento por mês e ano (heatmap)
- Faturamento por categoria, subcategoria e região

### Lucratividade
- Lucro total por ano
- Margem de lucro por categoria
- Produtos mais lucrativos e com maior prejuízo

### Análise de Móveis (Furniture)
- Margem de lucro por subcategoria
- Impacto do desconto no lucro
- Identificação do ponto de virada do prejuízo

### Clientes
- Top 10 clientes que mais compraram
- Top 10 clientes mais lucrativos
- Segmento mais lucrativo

### Análise Regional
- Região com maior faturamento e lucro
- Estados com maior prejuízo

### Correlação
- Mapa de correlação entre Sales, Profit, Discount e Quantity

---

## Principais Descobertas

### Problema em Furniture
- Furniture tem a menor margem de lucro: **3.8%**
- Tables apresenta margem de **-14.8%** — vendendo com prejuízo
- Bookcases apresenta margem de **-12.7%** — vendendo com prejuízo
- O motivo: descontos excessivos — Tables com **26%** e Bookcases com **21%** de desconto médio

### Impacto do Desconto
- A partir de **30% de desconto** praticamente toda venda vira prejuízo
- O desconto **não aumenta as vendas** (correlação: -0.028)
- O desconto **destrói o lucro** (correlação: -0.22)
- A empresa está dando desconto sem retorno algum

### Desempenho por Categoria
| Categoria | Margem de Lucro |
|---|---|
| Technology | 15.6% |
| Office Supplies | 13.8% |
| Furniture | 3.8% |

---

## Ferramentas Utilizadas

- **Python 3.9**
- **Pandas** — manipulação e análise de dados
- **Seaborn** — visualizações estatísticas
- **Matplotlib** — gráficos e customizações

---

## Autor

Feito por **Arthur Villar** — estudante de Data Science.
