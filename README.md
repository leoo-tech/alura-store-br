# Análise de Desempenho: Alura Store 🏪

> Projeto do Desafio Alura (Python para Data Science) para análise de desempenho de 4 lojas e recomendação estratégica de venda, utilizando fundamentos nativos de Python.

---

## 1. O Propósito da Análise

O Sr. João, dono da rede de e-commerce "Alura Store", precisa vender uma de suas 4 lojas para levantar capital e investir em um novo negócio.

O objetivo deste projeto foi realizar uma análise de ponta a ponta (desde a extração até a visualização) para identificar a loja com o menor potencial estratégico, fornecendo uma recomendação clara e baseada em dados sobre qual unidade deveria ser vendida.

## 2. Estrutura do Projeto

Este repositório está organizado da seguinte forma:

* **`README.md`**: Este arquivo, documentando todo o projeto.
* **`AluraStoreBrasil.ipynb`**: O notebook Jupyter contendo todo o código-fonte da análise. Ele inclui:
    * A extração dos dados (usando Pandas).
    * Todas as funções "raiz" (`def`, `for`, `if`) para calcular as 5 métricas.
    * Os 3 gráficos distintos (Barra, Pizza, Dispersão) gerados com `matplotlib`.
    * O relatório final em Markdown.
* **`/graficos`** (Opcional): <img width="921" height="632" alt="download (1)" src="https://github.com/user-attachments/assets/a0156a5e-f9d8-4ab0-beec-fcb1b78c3bfa" />


## 3. Exemplos de Gráficos e Insights Obtidos

A análise inicial apontou a **Loja 4** como a de pior faturamento. No entanto, a investigação revelou que ela era um "ativo oculto".

**A Reviravolta Geográfica:**
O insight decisivo veio da análise de geolocalização (colunas 'lat' e 'lon'). O gráfico de dispersão mostrou que as Lojas 1, 2 e 3 eram operações locais, enquanto a **Loja 4 (vermelha) era a única com distribuição NACIONAL**.

<img width="1024" height="863" alt="download" src="https://github.com/user-attachments/assets/9755b97f-aec1-4e3f-a1c7-d9936d7faf2c" />

**Outros Insights:**
* A **Loja 1** (maior faturamento) tinha a **pior avaliação** (3.98 estrelas) e o **frete mais caro**.
* A **Loja 4** (pior faturamento) tinha uma **boa avaliação** (4.00) e o **frete mais barato**.

**Recomendação Final:** Vender a **Loja 1**. Ela representa um risco (clientes insatisfeitos, logística cara) e tem alcance limitado. A Loja 4 é o ativo mais estratégico, com a melhor logística e alcance nacional.

## 4. Instruções para Executar o Notebook

1.  Clone este repositório (`git clone ...`).
2.  Abra o notebook `AluraStoreBrasil.ipynb` em um ambiente que leia Jupyter Notebooks (recomendado: **Google Colab**).
3.  No Google Colab, vá ao menu "Ambiente de execução".
4.  Clique em **"Executar tudo"**.
5.  O notebook irá carregar os dados dos CSVs, executar todas as funções de análise "raiz", gerar os 3 gráficos e exibir o relatório final no final.
