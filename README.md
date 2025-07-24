# Análise de Business Intelligence do Mercado de Airbnb em Nova York

## 📊 Dashboard Final

![Dashboard Final do Projeto Airbnb](dashboard-airbnb.png)


---

## 🎯 Objetivo do Projeto

Este projeto foca na exploração e análise de dados sobre a disponibilidade de quartos no Airbnb em Nova York. Utilizando ferramentas e conceitos de Business Intelligence (BI), o objetivo é revelar padrões de mercado, identificar oportunidades para anfitriões e aprimorar a tomada de decisões estratégicas.

---

## 🚀 Principais Insights e Conclusões

A análise dos dados permitiu extrair quatro conclusões principais sobre o mercado de Airbnb em NY:

1.  **Alta Competitividade no Segmento Econômico:** O mercado é dominado por uma vasta oferta de anúncios com preços abaixo de $150/noite, indicando um cenário de alta competição onde a diferenciação é crucial.
2.  **Concentração Geográfica:** A grande maioria dos anúncios está localizada nos bairros de Manhattan e Brooklyn, os principais centros turísticos e de negócios da cidade.
3.  **Preferência por Privacidade:** "Apartamentos/Casas Inteiras" e "Quartos Privados" compõem mais de 95% da oferta, mostrando uma baixa demanda ou oferta por espaços compartilhados.
4.  **Qualidade de Dados como Desafio Crítico:** O sucesso da análise dependeu de um processo robusto e iterativo de limpeza e padronização dos dados, que originalmente apresentavam múltiplas inconsistências.

---

## 🛠️ Ferramentas e Tecnologias Utilizadas

* **Google BigQuery:** Serviu como Data Warehouse para armazenar as tabelas e realizar transformações finais com SQL.
* **Google Colab (Python | Pandas):** Utilizado para o processo de limpeza profunda (Data Cleaning) e padronização dos dados brutos.
* **Power BI:** Ferramenta principal para modelagem de dados, criação de métricas (DAX) e desenvolvimento do dashboard interativo.
* **PowerPoint:** Usado para o design e prototipação do layout do dashboard.
* **Google Gemini:** Empregado como assistente de IA para orientação, debugging e formulação de insights.

---

## ⚙️ Processo de Análise e Transformação de Dados

O projeto seguiu um fluxo de trabalho completo de BI:

1.  **Limpeza e Preparação (Python):** Os dados brutos em CSV foram tratados no Google Colab para corrigir tipos, padronizar textos (`lower`, `trim`, `regexp_replace`) e tratar valores nulos.
2.  **Armazenamento e Transformação (BigQuery):** Os arquivos limpos foram carregados no BigQuery. Consultas SQL (`CREATE OR REPLACE TABLE`) foram usadas para aplicar as transformações finais e criar um conjunto de tabelas padronizadas.
3.  **Modelagem (Power BI):** O Power BI foi conectado às tabelas finais no BigQuery, onde foi construído um Modelo Estrela para relacionar as tabelas de fatos e dimensão.
4.  **Criação de Métricas (DAX):** As principais métricas do dashboard foram calculadas com DAX. Exemplo:
    ```dax
    Total de Reviews = SUM('reviews_final'[number_of_reviews])
    ```
5.  **Visualização e Storytelling:** Os dados foram apresentados em um dashboard interativo projetado para contar a história do mercado de Airbnb em NY, respondendo às principais perguntas de negócio.


## 🔗 Links de Interesse
- **[Google Colab projeto](https://colab.research.google.com/drive/1_ISjJgGiUgCNHuxa7onBCF8pVPVf3ljq?usp=sharing)**
- **[Ficha técnica completa no Notion](https://www.notion.so/Ficha-t-cnica-rota-de-aprendizagem-Business-Intelligence-BI-22d6dbae3c968056832fd01a479f7781?source=copy_link)**

---
## Contato

Gabriela Albuquerque  
[LinkedIn](https://www.linkedin.com/in/gabriela-cdeallbuquerque/) | [Portfólio](https://github.com/gabrielacalbuquerque)
