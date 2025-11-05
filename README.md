# Análise de Desempenho: Alura Store 🏪

> Projeto do Desafio Alura (Python para Data Science) para análise de desempenho de 4 lojas e recomendação estratégica de venda, utilizando fundamentos nativos de Python.

---

## 1. O Desafio

O Sr. João, dono da rede de e-commerce "Alura Store", precisa vender uma de suas 4 lojas para levantar capital e investir em um novo negócio.

Como Analista de Dados, minha missão foi realizar uma análise de ponta a ponta para identificar a loja com o menor potencial estratégico, fornecendo uma recomendação clara e baseada em dados sobre qual unidade deveria ser vendida.

## 2. Metodologia: O "Modo Raiz"

O foco principal deste desafio foi aplicar os fundamentos nativos do Python (`list`, `dict`, `for`, `if`, `def`) para realizar toda a manipulação e análise dos dados.

A biblioteca `pandas` foi utilizada estritamente para a extração inicial dos dados (carregar os 4 arquivos CSV), e o `matplotlib` foi usado para a visualização. Todo o "motor" da análise (cálculos, contagens, médias) foi feito em Python puro.

## 3. Análises Realizadas

Para fornecer uma recomendação completa, as seguintes métricas foram investigadas:

1.  **Faturamento Total:** O valor total vendido por cada loja.
2.  **Vendas por Categoria:** As categorias mais e menos populares em cada loja.
3.  **Média de Avaliação:** A satisfação média dos clientes (1-5 estrelas).
4.  **Produtos Mais/Menos Vendidos:** Um ranking de produtos específicos.
5.  **Frete Médio:** O custo logístico médio por venda.
6.  **(EXTRA) Análise Geográfica:** Um estudo da distribuição de vendas por latitude e longitude.

## 4. Principais Insights & A Reviravolta 🕵️‍♀️

A análise inicial apontou para um suspeito óbvio, mas a investigação mais profunda revelou um "ativo oculto":

* **Insight 1 (O Suspeito):** A **Loja 4** apresentou o **pior faturamento** de todas (R$ 1.38M), sendo a candidata óbvia para a venda.
* **Insight 2 (A Dúvida):** No entanto, a Loja 4 mostrou ter o **frete médio mais barato** da rede (R$ 31.28) e uma **avaliação de clientes (4.00)** superior à da Loja 1 (3.98), que era a que mais faturava.
* **Insight 3 (A Reviravolta):** O gráfico de análise geográfica foi a descoberta decisiva. Ele mostrou que as Lojas 1, 2 e 3 são operações **locais/regionais**, com vendas super concentradas. A **Loja 4 (vermelha) é a única com distribuição e logística de alcance NACIONAL**, vendendo para o Brasil inteiro.

<img width="1024" height="863" alt="download" src="https://github.com/user-attachments/assets/036e8deb-5174-4163-93b7-819e092fb375" />

## 5. Recomendação Final

**Recomendação:** Vender a **Loja 1**.

**Justificativa:**
A Loja 1, apesar do faturamento alto, representa o maior risco e o menor potencial de escala. Seus problemas são:
1.  **A Pior Satisfação do Cliente (3.98):** Vender uma loja com clientes insatisfeitos é uma decisão de saneamento de portfólio.
2.  **Logística Cara (Frete de R$ 34.69):** É a operação mais custosa por venda.
3.  **Alcance Geográfico Limitado:** É um negócio local, sem a infraestrutura de escala.

A **Loja 4**, por outro lado, é o **ativo mais estratégico** da rede. Seu faturamento é "baixo" por estar pulverizado nacionalmente, mas ela possui a melhor logística (frete barato), clientes satisfeitos e uma infraestrutura de alcance nacional. Vender a Loja 4 seria vender o ativo com maior potencial de crescimento futuro.

## 6. Como Executar

1.  Clone este repositório.
2.  Abra o notebook `AluraStoreBrasil.ipynb` no Google Colab.
3.  No menu, clique em "Ambiente de execução" > "Executar tudo" para ver todas as análises, gráficos e o relatório final.
