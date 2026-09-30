# 📌 MVP - [Análise de Sinistros e Frota no Brasil]

## 🎯 Objetivo do MVP
> Desenvolver uma primeira versão da solução de análise de segurança viária no Brasil, para permitir a visualização e comparação das taxas de mortes e sinistros, da gravidade das ocorrências por UF e Região e da participação de veículos de carga nos sinistros.

Qual problema resolvido?
A dificuldade de visualizar e comparar, de forma integrada, os dados de segurança viária entre os diferentes estados e regiões do Brasil, especialmente em relação às taxas de mortes e sinistros, à gravidade das ocorrências e à participação de veículos de carga.

Quais hipóteses serão validadas?
A representação dos dados por meio de gráficos e mapas facilita a comparação entre estados e regiões.

Os indicadores selecionados permitem observar diferenças na segurança viária entre as localidades.

A visualização dos dados auxilia o analista na interpretação das ocorrências.

Qual valor será entregue ao usuário final?
Uma visualização inicial dos principais indicadores de segurança viária, permitindo ao usuário analisar e comparar os dados de forma mais clara e visual.


---

## 📝 Descrição da Solução
> A solução consiste na coleta, organização, tratamento e análise de dados públicos relacionados à população, frota de veículos e sinistros de trânsito.

Os dados serão tratados utilizando ferramentas como Python, Google Colab, Power BI e GitHub, permitindo a criação de análises e visualizações que auxiliem na interpretação dos dados.

O MVP será desenvolvido de forma incremental, dividido em Sprints, começando pelas análises de taxas, população, frota e severidade dos sinistros.

Funcionalidades principais
Consolidação de dados populacionais por UF/região;
Consolidação de dados de frota por UF/região;
Cálculo de taxas de mortes por 100 mil habitantes;
Cálculo de taxas de sinistros por 10 mil veículos;
Comparação entre regiões e com a média nacional;
Análise da severidade dos sinistros;
Visualização dos dados por meio de gráficos e mapas.

## Limitações conhecidas

O MVP será desenvolvido utilizando dados públicos disponíveis nas fontes selecionadas pelo grupo;
A disponibilidade e o período dos dados podem limitar algumas análises;
As funcionalidades mais específicas, como análise de PPD, veículos pesados e densidade de sinistros, serão desenvolvidas nas Sprints posteriores. 

---

## 👥 Personas / Usuários-Alvo
- **Analista do ONSV:** Profissional responsável por analisar dados relacionados à segurança viária e utilizar informações estatísticas para identificar padrões, diferenças regionais e possíveis áreas de atenção. 
- **Gestor de Segurança Viária:** Usuário que necessita consultar dados de população, frota e sinistros para realizar estudos, análises e pesquisas relacionadas à segurança e ao transporte.

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

•	Comparar os indicadores regionais com a média brasileira;

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
- Prints de tela  
- Fluxos ou protótipos  
- Vídeo (MVP)  
