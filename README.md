# Plataforma de Inteligência Competitiva para o Varejo Supermercadista em Tempo Real

Este projeto implementa uma plataforma para análise de inteligência competitiva no setor supermercadista, focada em processamento em tempo real de dados de notas fiscais eletrônicas (NF-e) e geração de insights acionáveis através de um sistema de agentes autônomos.

## Funcionalidades Principais

- **Geração de XMLs NF-e simulados:** Criação de dados sintéticos para testes e demonstrações.
- **Leitura e processamento de NF-e:** Ingestão e extração de dados de arquivos XML.
- **Cálculo de KPIs (Preço, Margem, Mix):** Análise quantitativa dos dados processados.
- **Geração de gráficos e análise de dados:** Visualização e interpretação dos resultados.
- **Sistema de 15 Agentes Autônomos (6 Camadas):** Arquitetura modular para processamento e análise inteligente.
- **Interface Conversacional (Telegram) + Dashboards:** Formas de interação e visualização dos insights.

## Estrutura do Projeto (Sistema de Agentes Autônomos)

O sistema é baseado em uma arquitetura de 6 camadas com 15 agentes autônomos, orquestrados para processar dados, calcular KPIs, realizar análises e gerar recomendações.

1.  **CAMADA 1 - Ingestão:** Agentes responsáveis por ler e validar os dados de entrada (XML Parser, Data Validator).
2.  **CAMADA 2 - Processamento:** Agentes que agregam, calculam KPIs e enriquecem os dados (Aggregator, Calculator, Enricher).
3.  **CAMADA 3 - Análise (Paralela):** Agentes especializados em diferentes tipos de análise (Price Analyst, Margin Analyst, Mix Analyst, Competitive Analyst).
4.  **CAMADA 4 - Recomendações:** Agente que consolida as análises e gera recomendações priorizadas (Recommender).
5.  **CAMADA 5 - Interface:** Agentes para construir interfaces e relatórios (Dashboard Builder, Report Builder, Telegram Interface).
6.  **CAMADA 6 - Orquestração:** Agente mestre que coordena o fluxo de trabalho e gerencia o estado (Orchestrator, Memory Agent).

## Como Utilizar

1.  Abra o notebook AGROI2A2_PI_VAREJO.ipynb` no Google Colab ou em um ambiente compatível com Jupyter.
2.  Execute as células sequencialmente para:
    *   Instalar as dependências.
    *   Gerar arquivos XML simulados.
    *   Processar os XMLs e gerar DataFrames.
    *   Executar o sistema de agentes autônomos.
    *   Visualizar os resultados da análise e as recomendações.
    *   Testar a interação via Telegram simulada.
3.  Explore as variáveis geradas, como `df_notas`, `df_itens`, `analysis_results` e o objeto `orchestrator` para interagir com o sistema.

## Próximos Passos Sugeridos

- Integrar com a API oficial do Telegram Bot para interação real.
- Treinar modelos de NLU (Natural Language Understanding) para aprimorar a interface conversacional.
- Conectar o sistema a uma base de dados real de NF-e.
- Desenvolver um dashboard web interativo para visualização em tempo real.
- Otimizar a performance dos agentes e do fluxo de orquestração.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença
MIT License
