

# Análise Financeira Empresarial — Superstore

![Python](https://img.shields.io/badge/Python-3.9-blue?style=flat-square&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat-square&logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4c72b0?style=flat-square)
![Status](https://img.shields.io/badge/Status-Concluído-green?style=flat-square)

> **Uma rede de lojas americana fatura milhões por ano — mas será que está realmente lucrando?**
> Esta análise investiga onde o dinheiro está sendo perdido e por quê.

---

## O Problema

A Superstore é uma rede de lojas com operações em todo os Estados Unidos. Com mais de **9.994 pedidos entre 2014 e 2017**, a empresa parece saudável à primeira vista. Mas ao analisar os dados com mais profundidade, um problema grave surge: **uma categoria inteira está destruindo o lucro da empresa.**

---

## A Investigação

### Passo 1 — O faturamento cresce, mas o lucro acompanha?

Ao analisar o faturamento por ano, a empresa parece estar crescendo consistentemente. Porém, ao comparar com o lucro, percebemos que o crescimento de vendas não se traduz proporcionalmente em lucro.

### Passo 2 — Qual categoria está com problema?

Ao calcular a margem de lucro por categoria, o resultado é claro:

| Categoria | Margem de Lucro |
|---|---|
| Technology | 15.6% |
| Office Supplies | 13.8% |
| **Furniture** | **3.8%** |

Furniture (Móveis) tem uma margem alarmantemente baixa. Para uma empresa, uma margem de 3.8% significa que de cada R$100 vendidos, apenas R$3,80 viram lucro.

### Passo 3 — O que há dentro de Furniture?

Investigando as subcategorias, o problema fica ainda mais grave:

| Subcategoria | Margem de Lucro |
|---|---|
| Furnishings | +13.7% |
| Chairs | +4.4% |
| **Bookcases** | **-12.7%** |
| **Tables** | **-14.8%** |

**Tables e Bookcases estão sendo vendidas com prejuízo.** Ou seja, quanto mais a empresa vende esses produtos, mais dinheiro ela perde.

### Passo 4 — Qual é a causa raiz?

Analisando o desconto médio por subcategoria:

| Subcategoria | Desconto Médio |
|---|---|
| **Tables** | **26.1%** |
| **Bookcases** | **21.1%** |
| Chairs | 17.0% |
| Furnishings | 13.8% |

Os produtos com maior prejuízo são exatamente os que recebem os maiores descontos. E o pior: ao analisar a correlação entre desconto e vendas, descobrimos que o desconto **não aumenta as vendas** (correlação: -0.028). A empresa está simplesmente jogando dinheiro fora.

### Passo 5 — Qual é o ponto de virada?

A análise do gráfico de dispersão (Desconto vs Lucro) revela que a partir de **30% de desconto**, praticamente toda venda de Furniture se torna prejuízo.

---

## Conclusão e Recomendações

A Superstore tem um problema sério e específico: **descontos excessivos em Tables e Bookcases estão destruindo a lucratividade de toda a categoria Furniture.**

**Recomendações:**

- Limitar descontos em Tables e Bookcases a no máximo 20%
- Revisar a política de descontos — os dados mostram que descontos não aumentam vendas
- Focar esforços de vendas em Technology e Office Supplies, que têm margens saudáveis
- Investigar se os fornecedores de Tables e Bookcases podem oferecer preços melhores

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

- Faturamento anual e sazonalidade mensal
- Margem de lucro por categoria e subcategoria
- Impacto do desconto no lucro (causa raiz do problema)
- Top 10 produtos mais lucrativos e com maior prejuízo
- Top 10 clientes mais valiosos
- Desempenho por segmento e região
- Mapa de correlação entre variáveis numéricas

---

## Ferramentas Utilizadas

- **Python 3.9** — linguagem principal
- **Pandas** — manipulação e análise de dados
- **Seaborn** — visualizações estatísticas
- **Matplotlib** — gráficos e customizações

---



## Autor

**Arthur Villar** — Estudante de Data Science


