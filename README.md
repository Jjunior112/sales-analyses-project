# Contexto Inicial dos Dados

## 1. Visão geral

Este projeto tem como objetivo analisar uma base de dados de vendas de uma empresa fictícia, utilizando informações comerciais, financeiras, geográficas e de clientes para identificar padrões de comportamento, oportunidades de crescimento e pontos de atenção relacionados à performance das vendas.

A base contempla **10.000 registros de vendas**, distribuídos igualmente entre os anos de **2021, 2022, 2023, 2024 e 2025**, permitindo análises históricas e comparativas ao longo de cinco anos.

Os dados foram estruturados de forma a representar diferentes cenários comerciais, considerando variações de **sazonalidade, regiões, estados, produtos, segmentos de clientes e canais de venda**.

---

## 2. Período analisado

O período considerado no projeto compreende:

* **2021**
* **2022**
* **2023**
* **2024**
* **2025**

Cada ano possui **2.000 registros**, totalizando 10.000 vendas.

A existência de cinco anos de histórico permite avaliar:

* Evolução do faturamento;
* Crescimento ou redução das vendas;
* Variação da margem de lucro;
* Comportamento dos diferentes segmentos;
* Evolução das regiões;
* Desempenho dos produtos;
* Sazonalidade;
* Mudanças no comportamento dos canais de venda.

---

## 3. Estrutura dos dados

Cada registro representa uma **venda**, contendo informações relacionadas à transação, ao cliente, à localização, ao produto e aos resultados financeiros.

As principais dimensões disponíveis são:

### Venda

* `id_venda`
* `data`
* `ano`
* `mês`
* `dia`

### Cliente

* `id_cliente`
* `customer_segment`

Os clientes estão divididos em três segmentos:

* **Consumidor Final**
* **Pequenas Empresas**
* **Corporativo**

Os segmentos possuem comportamentos comerciais diferentes, principalmente em relação ao volume de vendas e ao potencial de faturamento.

### Localização

* `regiao`
* `estado`

A base contempla as regiões:

* Sudeste
* Sul
* Nordeste
* Centro-Oeste

Essa dimensão permite investigar diferenças de desempenho entre mercados e identificar regiões com maior ou menor potencial comercial.

### Produtos

* `produto_categoria`
* `produto_nome`

Os produtos pertencem a diferentes categorias e apresentam características distintas de preço, volume de vendas, receita e rentabilidade.

### Comercial

* `canal_venda`
* `quantidade`
* `preco_unitario`
* `pct_desconto`

Os canais disponíveis permitem comparar o desempenho entre **E-commerce** e **Loja Física**.

### Financeiro

* `gross_revenue`
* `discount_value`
* `net_revenue`
* `cost`
* `profit`
* `margin_pct`

Essas variáveis permitem analisar não apenas o volume de vendas, mas também a capacidade de geração de receita e lucro.

---

## 4. Características comerciais

Os dados foram estruturados para representar um cenário comercial com diferentes níveis de potencial.

### Segmentos

O segmento **Corporativo** apresenta, de forma geral, maior potencial de volume e faturamento.

**Pequenas Empresas** apresenta comportamento intermediário, enquanto **Consumidor Final** tende a apresentar menor volume por venda.

Essa diferenciação permite realizar análises como:

* Qual segmento gera mais receita?
* Qual segmento apresenta maior margem?
* O maior volume também representa maior rentabilidade?
* Quais produtos são mais relevantes para cada segmento?
* Como os segmentos evoluíram ao longo dos anos?

---

## 5. Diferenças regionais

As regiões apresentam diferentes níveis de participação e potencial comercial.

O objetivo é permitir análises que ultrapassem a simples identificação da região com maior faturamento.

É possível investigar:

* Receita por região;
* Lucro por região;
* Margem média;
* Volume de vendas;
* Produtos mais vendidos por região;
* Segmentos predominantes;
* Evolução regional ao longo dos anos;
* Estados com maior potencial;
* Regiões com crescimento acima ou abaixo da média.

Dessa forma, uma região com alto faturamento não necessariamente será considerada a melhor região caso apresente baixa margem ou baixo crescimento.

---

## 6. Sazonalidade

A base incorpora padrões sazonais ao longo do ano.

Determinados períodos apresentam maior potencial de vendas, especialmente nos meses associados a campanhas comerciais e ao aumento natural da demanda no final do ano.

Essa característica permite investigar:

* Meses com maior volume de vendas;
* Meses com maior faturamento;
* Meses com maior lucro;
* Variação da margem durante períodos sazonais;
* Diferenças de sazonalidade entre segmentos;
* Diferenças de sazonalidade entre regiões;
* Produtos mais sensíveis à sazonalidade.

A análise mensal também pode ser comparada entre os cinco anos para identificar se determinados padrões são recorrentes ou específicos de um período.

---

## 7. Potencial dos produtos

Os produtos possuem diferentes níveis de participação, preço e volume.

Isso possibilita classificar o portfólio considerando diferentes perspectivas, como:

* Produtos com maior faturamento;
* Produtos com maior quantidade vendida;
* Produtos com maior lucro;
* Produtos com maior margem;
* Produtos de alto volume e baixa margem;
* Produtos de baixo volume e alta margem;
* Produtos com crescimento ao longo dos anos.

Essa abordagem evita considerar apenas o produto mais vendido como necessariamente o produto mais estratégico.

---

## 8. Objetivo da análise

O objetivo principal do projeto é transformar os dados de vendas em **informações capazes de apoiar decisões comerciais**.

A análise buscará responder perguntas como:

### Performance

* Como as vendas evoluíram entre 2021 e 2025?
* Qual foi o crescimento anual da receita?
* Como o lucro e a margem evoluíram?

### Clientes

* Qual segmento apresenta maior potencial?
* Quais segmentos geram maior receita?
* Existe diferença significativa de rentabilidade entre os segmentos?

### Produtos

* Quais produtos possuem maior participação nas vendas?
* Quais produtos são mais lucrativos?
* Existem produtos com alto volume, mas baixa margem?

### Geografia

* Quais regiões apresentam melhor desempenho?
* Quais estados possuem maior potencial?
* Existem regiões crescendo acima da média?

### Sazonalidade

* Quais são os períodos de maior demanda?
* O comportamento sazonal se repete ao longo dos anos?
* Quais segmentos e produtos são mais influenciados pela sazonalidade?

### Canais

* Qual canal apresenta maior faturamento?
* Qual canal possui melhor margem?
* O comportamento dos clientes varia de acordo com o segmento e o canal?

---

## 9. Principais indicadores

Entre os principais KPIs que podem ser construídos estão:

* **Faturamento bruto**
* **Descontos concedidos**
* **Faturamento líquido**
* **Custo**
* **Lucro**
* **Margem (%)**
* **Quantidade vendida**
* **Ticket médio**
* **Receita por cliente**
* **Lucro por cliente**
* **Crescimento anual (%)**
* **Participação por região**
* **Participação por segmento**
* **Participação por produto**
* **Participação por canal**

---

## 10. Abordagem analítica

A análise será conduzida de forma exploratória e posteriormente orientada à geração de insights.

O fluxo proposto é:

**Dados → Tratamento → Exploração → KPIs → Segmentação → Análise temporal → Identificação de padrões → Insights → Recomendações**

O foco não será apenas apresentar indicadores, mas compreender **por que os resultados acontecem** e quais fatores estão associados à performance comercial.

---

## 11. Pergunta central do projeto

> **Quais segmentos, produtos, regiões e períodos apresentam maior potencial de geração de receita e lucro, e como esses fatores evoluíram entre 2021 e 2025?**

A partir dessa pergunta, as análises poderão identificar oportunidades de crescimento, pontos de atenção e possíveis direcionamentos para decisões comerciais.

---

O resultado esperado é um projeto de análise de dados que demonstre não apenas capacidade técnica de manipulação e visualização de dados, mas também capacidade de **interpretar resultados e convertê-los em recomendações de negócio**.
