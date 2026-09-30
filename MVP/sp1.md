# 📌 MVP - [Análise de Sinistros e Frota no Brasil]

## 🎯 Objetivo do MVP
> Desenvolver uma primeira versão da solução de análise de segurança viária no Brasil, para permitir a visualização e comparação das taxas de mortes e sinistros, da gravidade das ocorrências por UF e Região e da participação de veículos de carga nos sinistros.

- Qual problema resolvido?
A dificuldade de visualizar e comparar, de forma integrada, os dados de segurança viária entre os diferentes estados e regiões do Brasil, especialmente em relação às taxas de mortes e sinistros, à gravidade das ocorrências e à participação de veículos de carga.

- Quais hipóteses serão validadas?
A representação dos dados por meio de gráficos e mapas facilita a comparação entre estados e regiões.

Os indicadores selecionados permitem observar diferenças na segurança viária entre as localidades.

A visualização dos dados auxilia o analista na interpretação das ocorrências.

- Qual valor será entregue ao usuário final?
Uma visualização inicial dos principais indicadores de segurança viária, permitindo ao usuário analisar e comparar os dados de forma mais clara e visual.


---

## 📝 Descrição da Solução

> Será desenvolvida uma primeira versão da solução de análise de segurança viária utilizando os dados. Nesta etapa, os dados serão tratados e organizados para gerar duas visualizações gráficas e mapas por UF e Região, permitindo analisar diferentes aspectos dos sinistros de trânsito no Brasil.

- Funcionalidades principais

Gráfico relacionado às taxas de mortes e/ou sinistros;

Gráfico relacionado aos sinistros envolvendo veículos de carga;

Mapas para visualização dos dados por UF e Região;

Representação da gravidade/severidade dos sinistros;

Comparação entre diferentes estados e regiões.


## Limitações conhecidas
Dependência da qualidade das bases: possíveis inconsistências, diferenças de preenchimento ou ausência de informações nas bases podem influenciar os resultados apresentados.

 Grande volume de dados: a quantidade de informações disponibilizadas exigiu um processo significativo de organização, filtragem e tratamento antes de sua utilização nas visualizações.

---

## 👥 Personas / Usuários-Alvo
- **Analista do ONSV:** Profissional responsável por analisar dados relacionados à segurança viária e acompanhar os indicadores de sinistros no Brasil. 
Necessidades: Consultar dados de sinistros de trânsito, comparar indicadores entre UFs e Regiões, analisar taxas de mortes e sinistros;

Avaliar a gravidade das ocorrências;

Verificar a participação de veículos de carga nos sinistros.
- **Gestor de Segurança Viária:** Profissional que utiliza informações e indicadores de segurança viária para acompanhar o cenário dos sinistros e apoiar o planejamento de ações.


Necessidades: Consultar informações consolidadas sobre os sinistros, comparar resultados entre estados e regiões, identificar diferenças nos níveis de gravidade das ocorrências e acompanhar indicadores relacionados a mortes, sinistros e veículos de carga.

---

## 🔑 User Stories (Backlog do MVP)
| Rank | Prioridade | User Story | Estimativa | Sprint |
| :---: | :---: | :--- | :---: | :---: |
| **1** | Alta | **Como** analista do ONSV, **quero** visualizar as taxas de mortes por 100 mil hab. e sinistros por 10 mil veículos, **para que** eu compare o desempenho regional com a média do Brasil. |40  | 1 |
| **2** | Alta | **Como** analista do ONSV, **quero** mapear a gravidade das ocorrências de sinistros por UF e Região, **para que** eu possa comparar os índices de severidade entre os diferentes estados. | 40 | 1 |
| **3** | Média | **Como** analista da ONSV, **quero** visualizar a taxa de sinistro com veículos de cargas, **para que** possa entender qual a relação com total de sinistro | 20 | 1 |
---

## 📅 Sprint(s) Relacionadas
| Sprint | Entregas Principais                          | Status   |
|--------|----------------------------------------------|----------|
| 01     | Visualização das taxas de mortes e sinistros; consolidação de dados populacionais e de frota por UF/região; mapeamento da severidade dos sinistros por UF/região.                        | Concluída|
| 02     | Análise da distância entre sinistros com veículos pesados e PPD; análise estatística entre frota pesada e sinistros fatais; visualização da densidade de sinistros de veículos pesados no Sudeste..  | Planejada|
| 03     | Visualização da classificação de letalidade dos sinistros em São José dos Campos; comparação das taxas de mortes e sinistros de São José dos Campos com a média do estado de São Paulo.  | Planejada|

---

## 📊 Critérios de Aceitação
- O MVP deverá permitir:
•	Consolidar dados populacionais por UF/região;

•	Consolidar dados de frota por UF/região;

•	Visualizar o crescimento da frota durante o período analisado;

•	Calcular as taxas de mortes por 100 mil habitantes;

•	Calcular as taxas de sinistros por 10 mil veículos;

•	Comparar os indicadores totais de sinistro com os indicadores de sinistros envolvendo veículos de carga;

•	Mapear a severidade dos sinistros por UF/região;

•	Apresentar os resultados de forma clara e visual;

•	Registrar os códigos, dados e evidências do desenvolvimento no GitHub.


---

## 📈 Métricas de Validação
- Número de usuários que testaram o MVP  
- Feedback qualitativo (positivo/negativo)  
- Indicadores de negócio (exemplo: % de adesão, redução de custo, etc.)  

---

## 🚀 Próximos Passos
- Melhorias planejadas após feedback  
- Ajustes de usabilidade  
- Expansão de funcionalidades para próximo incremento  

---

## 📂 Anexos / Evidências

<img width="1131" height="1600" alt="mapa mediadeseveriedade" src="https://github.com/user-attachments/assets/b5795318-451a-4929-8a47-fbebefba98fa" />

