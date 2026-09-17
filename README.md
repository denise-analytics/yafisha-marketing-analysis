# Análise de Marketing e Unit Economics — Y.Afisha

## Visão geral

Este projeto analisa o comportamento dos usuários, as vendas e a eficiência dos investimentos em marketing da plataforma Y.Afisha.

O estudo combina métricas de produto, análise de coortes e indicadores financeiros para identificar como os usuários interagem com a plataforma, quanto tempo levam para realizar a primeira compra e quais canais de aquisição geram melhor retorno.

## Objetivos

- Avaliar o nível de atividade e engajamento dos usuários.
- Analisar a duração e a frequência das sessões.
- Medir a retenção por coortes.
- Identificar o tempo necessário para a primeira compra.
- Avaliar a recorrência e o valor dos pedidos.
- Calcular o Lifetime Value (LTV).
- Comparar o custo de aquisição de clientes entre as fontes.
- Avaliar o retorno dos investimentos em marketing.
- Recomendar melhorias na distribuição do orçamento.

## Dados analisados

O projeto utiliza três conjuntos de dados:

| Arquivo | Conteúdo |
|---|---|
| `visits_log_us.csv` | Visitas, usuários, origem do tráfego, dispositivo e duração das sessões |
| `orders_log_us.csv` | Pedidos, compradores, datas e valores das transações |
| `costs_us.csv` | Investimentos diários por fonte de aquisição |

Os dados abrangem o período entre 2017 e 2018.

## Metodologia

A análise foi organizada em três áreas.

### Produto

Foram calculadas métricas de atividade e engajamento:

- DAU — usuários ativos diariamente;
- WAU — usuários ativos semanalmente;
- MAU — usuários ativos mensalmente;
- sessões por dia;
- duração das sessões;
- quantidade de sessões por usuário;
- retenção por coortes.

### Vendas

Foram analisados:

- tempo entre a primeira visita e a primeira compra;
- pedidos por usuário;
- receita por pedido;
- comportamento das coortes;
- Lifetime Value (LTV).

### Marketing

Foram avaliados:

- investimentos por fonte;
- custo de aquisição de clientes (CAC);
- retorno sobre o investimento;
- retorno acumulado por coorte;
- diferenças de desempenho entre os canais.

## Principais resultados

| Indicador | Resultado |
|---|---:|
| Mediana da duração das sessões | 5 minutos |
| Sessões com duração de até 14 minutos | 75% |
| Retenção média no mês seguinte | Aproximadamente 6,5% |
| Mediana até a primeira compra | 0 dias |
| Usuários que compraram em até 2 dias | 75% |
| Mediana da receita por pedido | Aproximadamente 2,5 |
| CAC médio geral | Aproximadamente 8 |
| Menor CAC | Fonte 9 — aproximadamente 4,87 |
| Maior CAC | Fonte 3 — aproximadamente 13,80 |

## Comportamento dos usuários

A atividade da plataforma cresceu durante o período analisado, com aumento das métricas DAU, WAU e MAU.

Entretanto, a maior parte dos usuários realizou apenas uma sessão. A mediana da duração foi de **5 minutos**, e 75% das sessões duraram até **14 minutos**.

A diferença entre usuários ativos diariamente, semanalmente e mensalmente indica que apenas uma parcela da base retorna com frequência.

## Retenção

A retenção apresentou uma queda acentuada após o primeiro mês.

Em média, aproximadamente **6,5% dos usuários retornaram no mês seguinte à aquisição**. Nos períodos posteriores, os percentuais permaneceram geralmente entre 2% e 5%.

Esse comportamento indica que a plataforma consegue atrair usuários, mas enfrenta dificuldades para mantê-los ativos e estimular compras recorrentes.

## Conversão e vendas

A conversão ocorreu principalmente nos primeiros contatos com a plataforma:

- a mediana até a primeira compra foi de **0 dias**;
- pelo menos metade dos compradores realizou a compra no mesmo dia da primeira visita;
- 75% converteram em até **2 dias**.

A receita por pedido apresentou distribuição assimétrica. A mediana ficou próxima de **2,5**, enquanto poucos pedidos de maior valor elevaram a média.

Os resultados mostram boa capacidade de conversão inicial, mas baixa recorrência de compras nos períodos seguintes.

## Lifetime Value

O LTV médio cresceu ao longo do ciclo de vida dos clientes, passando de aproximadamente **4,8 no mês inicial** para valores superiores a **10 nas coortes mais maduras**.

O crescimento foi mais intenso nos primeiros meses e desacelerou posteriormente. A diferença entre média e mediana indica que poucos usuários de maior valor elevam o resultado agregado.

O aumento sustentável do LTV depende principalmente da melhoria da retenção e da recorrência de compras.

## Custo de aquisição

O CAC apresentou diferenças importantes entre os canais:

| Fonte | CAC aproximado | Avaliação |
|---|---:|---|
| 9 | 4,87 | Menor custo |
| 10 | 5,41 | Baixo custo |
| 2 | 12,50 | Custo elevado |
| 3 | 13,80 | Maior custo |

A fonte 7 não apresentou CAC calculável porque não houve clientes convertidos registrados nessa origem.

O CAC não deve ser analisado isoladamente. Canais de menor custo precisam também gerar receita e retenção suficientes para justificar o investimento.

## Retorno dos investimentos

A fonte 1 apresentou o melhor retorno sobre o investimento.

As fontes 2, 5 e 9 operaram próximas ao ponto de equilíbrio, enquanto as fontes 3, 4 e 10 apresentaram retorno negativo no período analisado.

Nos primeiros meses após a aquisição, o retorno de marketing permaneceu predominantemente negativo. A recuperação ocorreu gradualmente e dependeu do valor acumulado pelos clientes ao longo do tempo.

A fonte 10 representa um exemplo importante: apesar de apresentar um dos menores custos de aquisição, seu retorno foi negativo. Isso demonstra que um CAC baixo não garante rentabilidade e reforça a necessidade de avaliar CAC, LTV e retorno de forma conjunta.

Esse resultado reforça que investir apenas em aquisição, sem melhorar retenção e monetização, pode comprometer a sustentabilidade do crescimento.

## Recomendações de negócio

- Priorizar canais que combinem CAC competitivo e retorno positivo.
- Reavaliar os investimentos nas fontes 3, 4 e 10.
- Investigar os fatores responsáveis pelo desempenho da fonte 1.
- Desenvolver estratégias de retenção após a primeira compra.
- Estimular recorrência por meio de campanhas segmentadas.
- Trabalhar no aumento do valor médio dos pedidos.
- Monitorar CAC, LTV e retorno de forma conjunta.
- Revisar periodicamente a distribuição do orçamento entre as fontes.

## Limitações

- Os dados representam um período específico entre 2017 e 2018.
- A análise identifica associações, mas não comprova causalidade.
- As fontes são representadas por identificadores numéricos, sem descrição dos canais.
- Não estão disponíveis informações sobre margem de lucro, categoria dos produtos ou perfil demográfico.
- Algumas coortes possuem períodos de observação menores que outras.
- A concentração de receita em poucos usuários pode influenciar médias e indicadores agregados.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Estrutura do repositório

```text
yafisha-marketing-analysis/
├── data/
│   ├── costs_us.csv
│   ├── orders_log_us.csv
│   └── visits_log_us.csv
├── notebooks/
│   └── marketing_analytics_yafisha.ipynb
├── .gitignore
├── README.md
└── requirements.txt
```

## Como executar o projeto

1. Clone o repositório:

```bash
git clone https://github.com/denise-analytics/yafisha-marketing-analysis.git
```

2. Acesse a pasta:

```bash
cd yafisha-marketing-analysis
```

3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Entre na pasta do notebook:

```bash
cd notebooks
```

5. Inicie o Jupyter Notebook:

```bash
jupyter notebook
```

Abra `marketing_analytics_yafisha.ipynb` e execute as células na ordem apresentada.

## Notebook

A análise completa, incluindo métricas de produto, coortes, LTV, CAC e retorno dos investimentos, está disponível em:

[Análise completa em Jupyter Notebook](notebooks/marketing_analytics_yafisha.ipynb)

## Autora

**Denise Duarte**  
Analista de Dados Júnior | Python | SQL | Excel | Power BI