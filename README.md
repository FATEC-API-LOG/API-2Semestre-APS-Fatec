# Aprendizado por Projeto Integrado (API)

Projeto baseado na metodologia ágil SCRUM, procurando desenvolver a Proatividade, Autonomia, Colaboração e Entrega de Resultados dos estudantes envolvidos

# Índice
* [Objetivo do Projeto](#objetivo-do-projeto)
* [Equipe](#Equipe)
* [Backlog do produto](#Product-Backlog)
* [Competências desenvolvidas](#competências-desenvolvidas)
* [Registro das Sprints](#Registro-das-Sprints)


# Projeto (API) 
Projeto pedagógico alicerçado na Metodologia API para ensino-aprendizado focado no desenvolvimento de competências e fundamentada nos pilares de aprendizado com problemas reais (RPBL), validação externa e mentalidade ágil. 
Uso de estratégias para entender o problema, conceber uma solução viável ao desenvolver e implementar o MVP seguido de sua operação (CDIO). 
Os resultados dos projetos devem obedecer ao Aviso Legal disponível no site da Fatec SJC com definição das datas do kickoff e das sprint

# Equipe

| Função | Nome | LinkedIn & GitHub |
| :---: | :--- | :---: |
| Product Owner | Tiago Mesquita | [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/tiago-mesquita-a2633a267?utm_source=share_via&utm_content=profile&utm_medium=member_ios) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/otiagomesquita) |
| Scrum Master | Luiz Augusto | [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/luiz-augusto-campos-886a3a369/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Luiz-A-Campos) |
| Team Member | Aldo Pereira | [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/aldo-pereira-a7aa9682?utm_source=share_via&utm_content=profile&utm_medium=member_android) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Aldus147) |
| Team Member | Ana Carolina | [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/ana-carolina-oliveira-da-silva-3b0047406?utm_source=share_via&utm_content=profile&utm_medium=member_android) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/anacoliveirasv11) |
| Team Member | Felipe Borges | [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/felipe-borges-46ab48326?utm_source=share_via&utm_content=profile&utm_medium=member_android) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Flspo) |
| Team Member | José Augusto | [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/josé-augusto-2b66743b0?utm_source=share_via&utm_content=profile&utm_medium=member_android) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/JoseAugustoV) |
| Team Member | Luiz Gustavo | [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/luiz-gustavo-bettoni-b6908b23b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/luizgustavobettoni7) |
| Team Member | Rita Carolina | [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/rita-carolina79?utm_source=share_via&utm_content=profile&utm_medium=member_ios) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/ritt4c) |

# Objetivo do Projeto

Os objetivos estabelecidos para esse projeto consistem em:

* Analisar a dinâmica e os padrões de sinistros de trânsito no Brasil entre 2015 e 2025, cruzando dados da PRF, DATASUS, frota e população para gerar indicadores epidemiológicos normalizados por Unidade Federativa;

* Desenvolver uma solução analítica integrada com scripts em Python (Google Colab) e dashboards interativos, permitindo a visualização de taxas de severidade, mapas temáticos de densidade em rodovias federais e filtros dinâmicos de alta granularidade;

* Avaliar o impacto logístico e os fatores de risco associados a veículos pesados e motocicletas, mapeando a desassistência por Pontos de Parada e Descanso (PPD) e correlacionando o crescimento da frota com sinistros fatais para subsidiar relatórios técnicos e políticas públicas.

# Tecnologias Utilizadas

* Jira Software
* Power BI
* Python (Colab)
* Microsoft Excel
* GitHub
* QGIS

# Product Backlog — Análise Integrada de Segurança Viária no Brasil (2015 - 2025)

| Rank | Prioridade | User Story | Estimativa | Sprint |
| :---: | :---: | :--- | :---: | :---: |
| **1** | Alta | **Como** analista do ONSV, **quero** visualizar as taxas de mortes por 100 mil hab. e sinistros por 10 mil veículos, **para que** eu compare o desempenho regional com a média do Brasil. |  | 1 |
| **2** | Média | **Como** analista do ONSV, **quero** mapear por UF/região, a gravidade da ocorrência dos sinistros, **para que** eu possa comparar os indices de severidade dos sinistros UF/região. |  | 1 |
| **3** | Alta | **Como** analista do ONSV, **quero** calcular e mapear a distância entre os sinistros com veículos pesados e os Pontos de Parada e Descanso (PPD), **para que** eu identifique trechos desassistidos e padrões de risco por fadiga no estado de São Paulo. |  | 2 |
| **4** | Média | **Como** analista do ONSV, **quero** analisar a correlação estatística entre o crescimento da frota pesada e o aumento de sinistros fatais em São Paulo, **para que** eu fundamente estudos de impacto logístico. |  | 2 |
| **5** | Alta | **Como** analista do ONSV, **quero** visualizar a densidade de sinistros de veículos pesados no sudeste dentro das rodovias federais (BRs),  **para que** eu localize visualmente os trechos rodoviários mais críticos e perigosos do estado. |  | 2 |
| **6** | Média | **Como** analista do ONSV, **quero** visualizar a quantidade de sinistros por classificação de letalidade (com vítimas fatais e não fatais) em São José dos Campos **para que** eu compreenda o impacto dessas colisões de forma clara e ágil. |  | 3 |
| **7** | Baixa | **Como** analista do ONSV, **quero** visualizar as taxas de mortes por 100 mil hab. e sinistros por 10 mil veículos, **para que** eu compare o desempenho de São José dos Campos com a média do estado de São Paulo. |  | 3 |
  
# Registro das Sprints

| Sprint            | Previsão   | Status   | Histórico |
|-------------------|------------|----------|-----------|
| 01                | 30/09/2026 | a fazer  | [MVP](MVP/sp1.md)  |
| 02                | 28/10/2026 | a fazer  | [MVP](MVP/sp2.md)  |
| 03                | 25/11/2026 | a fazer  | [MVP](MVP/sp3.md)  |
| Feira de Soluções | 03/12/2026 | a fazer  | [MVP](#)  |

