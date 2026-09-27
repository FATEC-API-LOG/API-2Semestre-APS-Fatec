# 📌 MVP - [Análise de Sinistros e Frota no Brasil]

## 🎯 Objetivo do MVP
> Desenvolver uma solução de análise de dados para o ONSV (Observatório Nacional de Segurança Viária), permitindo consolidar, visualizar e comparar informações relacionadas à população, frota de veículos e sinistros de trânsito.

O MVP tem como objetivo validar a utilização de dados públicos para:

Comparar taxas de mortes e sinistros entre regiões;
Consolidar dados populacionais e de frota por UF/região;
Identificar territórios com maior crescimento da frota;
Analisar a severidade dos sinistros por UF/região;
Apoiar a visualização de informações relevantes para estudos de segurança viária.

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

Limitações conhecidas
O MVP será desenvolvido utilizando dados públicos disponíveis nas fontes selecionadas pelo grupo;
A disponibilidade e o período dos dados podem limitar algumas análises;
As funcionalidades mais específicas, como análise de PPD, veículos pesados e densidade de sinistros, serão desenvolvidas nas Sprints posteriores. 

---

## 👥 Personas / Usuários-Alvo
- **Analista do ONSV:** Profissional responsável por analisar dados relacionados à segurança viária e utilizar informações estatísticas para identificar padrões, diferenças regionais e possíveis áreas de atenção. 
- **Persona 2:** Usuário que necessita consultar dados de população, frota e sinistros para realizar estudos, análises e pesquisas relacionadas à segurança e ao transporte.

---

## 🔑 User Stories (Backlog do MVP)
| ID  | User Story                                                                 | Prioridade | Estimativa |
|-----|-----------------------------------------------------------------------------|------------|------------|
| US1 | Como analista do ONSV, quero visualizar as taxas de mortes por 100 mil habitantes e sinistros por 10 mil veículos, para que eu compare o desempenho regional com a média do Brasil..         | Alta       | 5 pontos   |
| US2 | Como analista do ONSV, quero consolidar dados populacionais e número de frota por UF/região, para que seja viável visualizar territórios que tiveram maior aumento de frotas no Brasil durante esse período..         | Média      | 3 pontos   |
| US3 | Como analista do ONSV, quero mapear por UF/região a gravidade da ocorrência dos sinistros, para que eu possa comparar os índices de severidade dos sinistros por UF/região.         | Média      | 3 pontos   |
| US4 | Como analista do ONSV, quero calcular e mapear a distância entre os sinistros com veículos pesados e os Pontos de Parada e Descanso (PPD), para que eu identifique trechos desassistidos e padrões de risco por fadiga no estado de São Paulo.      | Média      | 3 pontos   |
| US5 | Como analista do ONSV, quero analisar a relação estatística entre o crescimento da frota pesada e o aumento de sinistros fatais em São Paulo, para que eu fundamente estudos de impacto logístico.       | Média      | 3 pontos   |
| US6 | Como analista do ONSV, quero visualizar a densidade de sinistros de veículos pesados no Sudeste dentro das rodovias federais (BRs), para que eu localize visualmente os trechos rodoviários mais críticos e perigosos da região.        | Média      | 3 pontos   |
| US7 | Como analista do ONSV, quero visualizar a quantidade de sinistros por classificação de letalidade (com vítimas fatais e não fatais) em São José dos Campos, para que eu compreenda o impacto dessas colisões de forma clara e ágil.     | Média      | 3 pontos   |
| US8 | Como analista do ONSV, quero visualizar as taxas de mortes por 100 mil habitantes e sinistros por 10 mil veículos, para que eu compare o desempenho de São José dos Campos com a média do estado de São Paulo.      | Média      | 3 pontos   |

---

## 📅 Sprint(s) Relacionadas
| Sprint | Entregas Principais                          | Status   |
|--------|----------------------------------------------|----------|
| 01     | Visualização das taxas de mortes e sinistros; consolidação de dados populacionais e de frota por UF/região; mapeamento da severidade dos sinistros por UF/região.                        | Em andamento|
| 02     | Análise da distância entre sinistros com veículos pesados e PPD; análise estatística entre frota pesada e sinistros fatais; visualização da densidade de sinistros de veículos pesados no Sudeste.
| 02     | Visualização da classificação de letalidade dos sinistros em São José dos Campos; comparação das taxas de mortes e sinistros de São José dos Campos com a média do estado de São Paulo.

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
