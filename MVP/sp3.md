# 📌 MVP 

## 🎯 Objetivo do MVP
* **Qual problema resolve?** A distorção na análise de segurança viária causada pelo uso exclusivo de números absolutos de acidentes. Municípios com grandes frotas (como São José dos Campos) lideram o volume bruto de colisões, enquanto municípios menores cortados pela Rodovia Presidente Dutra (BR-116) escondem riscos proporcionais severos devido ao intenso tráfego de passagem. Além disso, faltava uma visão consolidada e rápida do índice de severidade (UPS) para apoiar decisões de fiscalização e políticas públicas.
* **Qual hipótese será validada?** Ao normalizar a severidade dos sinistros (método UPS - Unidade Padrão de Severidade) pela frota média de carga local e disponibilizar painéis interativos por *User Story*, os analistas do ONSV conseguem identificar com maior justiça os trechos verdadeiramente críticos da BR-116 e compreender rapidamente o impacto das colisões em polos urbanos como São José dos Campos.
* **Qual valor será entregue ao usuário final?** Diagnóstico viário ágil, transparente e comparativo (Risco Real vs. Volume Bruto), permitindo priorizar fiscalização eletrônica, engenharia de tráfego e ações educativas onde o risco proporcional e a gravidade das ocorrências são mais críticos.

---

## 📝 Descrição da Solução
Aplicação web interativa (*Single-Page Application* em HTML5, Tailwind CSS e JavaScript/SVG) organizada diretamente pelo *Product Backlog* do projeto, integrando dados da PRF, Infosiga e Senatran (2019–2025) para entregar análises visuais das User Stories 7 e 8 (além da integração com os mapas estaduais das Sprints anteriores).

* **Funcionalidades principais incluídas:**
  * **Ranking de Risco Real na BR-116 (US 7):** Ordenação dinâmica dos 16 municípios do Vale do Paraíba cortados pela Dutra por *UPS / 10 mil veículos de carga/ano*, taxa de sinistros, mortalidade, UPS total e gravidade média.
  * **Filtros e Escopo Estatístico:** Separação entre municípios de frota estável ($\ge 330$ veículos) e frota pequena ($< 330$ veículos), além de busca por município e exportação dos dados filtrados em `.csv`.
  * **Matriz de Decisão e Perfil Espacial:** Gráfico de dispersão (*Risco Real vs. Severidade Bruta*) e linha geográfica sequencial do corredor (Jacareí $\rightarrow$ Queluz) com cards de diagnóstico e recomendações de políticas públicas por cidade.
  * **Painel de Severidade de São José dos Campos (US 8):** Decomposição visual do índice UPS de SJC (1.034 pontos), participação percentual de sinistros fatais, com feridos e danos materiais, e comparativo direto com os principais municípios do corredor.
* **Limitações conhecidas:**
  * Municípios com frota local muito reduzida ($< 330$ veículos de carga, como Lavrinhas e Canas) sofrem distorção estatística no denominador devido ao tráfego predominante de longa distância, exigindo sinalização de alerta na interface.
  * Em trechos limítrofes com poucos registros (ex.: Santa Branca e Silveiras), há dependência da precisão do georreferenciamento original (km/coordenadas) da base da PRF.
* **Escopo reduzido (somente o essencial para validar a ideia):**
  * Foco exclusivo nos dados históricos consolidados (2019–2025) sem ingestão em tempo real via API externa, utilizando processamento estático em memória no navegador para garantir carregamento instantâneo e validação imediata das regras de negócio (cálculo UPS e normalização por frota).

---

## 👥 Personas / Usuários-Alvo
* **Persona 1 — Analista de Dados e Segurança Viária do ONSV:** Profissional técnico que precisa cruzar bases de sinistros (PRF/Infosiga) e frota (Senatran) para produzir estudos embasados. **Necessidades e dores atendidas:** Elimina o trabalho manual em planilhas estáticas, evita conclusões enviesadas pelo tamanho da frota municipal e entrega métricas padronizadas (UPS/10k) prontas para relatórios.
* **Persona 2 — Gestor de Políticas Públicas e Planejamento de Fiscalização:** Tomador de decisão (órgãos de trânsito, concessionárias e autoridades rodoviárias) que define onde alocar radares, operações da PRF e obras de engenharia. **Necessidades e dores atendidas:** Visualiza rapidamente quais cidades precisam de controle de velocidade em trechos de passagem versus gestão de conflitos urbanos e travessias (como em SJC).

---

## 🔑 User Stories (Backlog do MVP)

| ID | Prioridade | User Story | Estimativa | Sprint |
| :--- | :--- | :--- | :---: | :---: |
| **7** | Média | **Como** analista do ONSV, **quero** visualizar um ranking dos municípios do Vale do Paraíba (SP) cortados pela Rodovia Presidente Dutra (BR-116), ordenado pelo risco real de acidentes, **para** que eu possa identificar de forma justa quais cidades concentram os trechos mais críticos e direcionar políticas de segurança viária e fiscalização. | 20 | 3 |
| **8** | Média | **Como** analista do ONSV, **quero** visualizar o índice de severidade em São José dos Campos, **para** que eu compreenda o impacto dessas colisões de forma clara e ágil. | 20 | 3 |

---

## 📅 Sprint(s) Relacionadas

| Sprint | Entregas Principais | Status |
| :---: | :--- | :---: |
| **01** | Levantamento de requisitos, definição da metodologia UPS (DENATRAN/DNIT) e estruturação das bases PRF, Infosiga e Senatran. | Concluído |
| **02** | Mapas espaciais estaduais (Distância de PPDs, Crescimento de Frota $\times$ Fatais e Densidade KDE — US 4, 5 e 6). | Concluído |
| **03** | Módulo de Risco Real da BR-116 no Vale do Paraíba (US 7), Painel de Severidade de São José dos Campos (US 8) e exportação CSV. | Concluído |

---

## 📊 Critérios de Aceitação
* **O MVP deve permitir que o usuário:**
  * Alterne entre as abas das *User Stories* e ordene o ranking dos 16 municípios da BR-116 pelo índice de Risco Real ($\text{UPS} / 10\text{ mil veículos/ano}$), filtrando por porte de frota ($\ge 330$ vs. $< 330$) e visualizando a diferença de posição em relação ao ranking bruto.
  * Inspecione de forma imediata o índice de severidade de São José dos Campos (1.034 UPS totais, média de 3,38 UPS/sinistro e distribuição entre danos materiais, feridos e óbitos) e exporte os dados filtrados em CSV.
* **O sistema deve registrar:**
  * Seleção de município ativo para atualização sincronizada entre o gráfico de barras, a matriz de dispersão, o perfil espacial do corredor e o painel de diagnóstico técnico/recomendações.
  * Preferência de visualização do usuário (alternância entre tema claro/escuro e exibição/ocultação das premissas metodológicas).
* **Métricas coletadas:**
  * Tempo de carregamento e renderização dos gráficos SVG no navegador ($< 1\text{s}$), taxa de utilização dos filtros de escopo estatístico e número de exportações CSV realizadas durante os testes.

---

## 📈 Métricas de Validação
* **Número de usuários que testaram o MVP:** Equipe interna do projeto (Product Owner, desenvolvedores e analistas) e avaliadores/stakeholders do ONSV durante a apresentação da Sprint 3.
* **Feedback qualitativo (positivo/negativo):** Validação da clareza visual na distinção entre municípios de passagem (ex.: Lavrinhas em 1º no risco real) e polos urbanos de alto volume bruto (ex.: SJC em 1º no UPS total e 15º no risco normalizado), além da facilidade de leitura da composição de gravidade em SJC.
* **Indicadores de negócio:** Redução do tempo de análise comparativa entre municípios do Vale do Paraíba e 100% de aderência às fórmulas oficiais de ponderação de severidade ($\text{UPS} = 1 \times \text{Danos} + 5 \times \text{Feridos} + 13 \times \text{Óbitos}$).

---

## 🚀 Próximos Passos
* **Melhorias planejadas após feedback:** Incorporar filtros temporais ano a ano (série histórica 2019–2025) para permitir a análise de tendência e evolução da severidade após intervenções viárias.
* **Ajustes de usabilidade:** Adicionar comparação lado a lado (*benchmarking* direto) entre dois municípios selecionados pelo analista e tooltips ainda mais detalhados nos gráficos de dispersão em telas menores (mobile).
* **Expansão de funcionalidades para próximo incremento:** Integrar os marcos quilométricos (km inicial e final) exatos de cada ocorrência da PRF no mapa interativo da BR-116 e automatizar a atualização das bases via pipeline Python conectado ao repositório.

---

## 📁 Anexos / Evidências
* **Prints de tela:** Capturas das interfaces de Ranking de Risco Real (US 7), Matriz de Decisão e Painel de Severidade de São José dos Campos (US 8).
* **Fluxos ou protótipos:** Aplicação web funcional consolidada no arquivo `painel_backlog_onsv.html`.
* **Vídeo (MVP):** Demonstração navegável dos filtros, inspeção de diagnósticos municipais e exportação de dados.
```[cite: 1, 2, 3, 4, 5]
