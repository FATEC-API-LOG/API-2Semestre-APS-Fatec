# 📌 MVP - [Análise de Sinistros e Frota no Brasil]

## 🎯 Objetivo do MVP

O propósito deste incremento (Sprint 2) é fornecer ao Observatório Nacional de Segurança Viária (ONSV) uma ferramenta analítica e geoespacial integrada para correlacionar sinistros envolvendo veículos pesados, a oferta de infraestrutura de descanso e a dinâmica da frota em circulação.

- **Qual problema resolve?**  
  A escassez de infraestrutura de suporte ao motorista profissional (desassistência de PPDs acima de 50 km) associada a sinistros causados por fadiga nas rodovias paulistas, aliada à ausência de visualização consolidada dos trechos mais críticos e do impacto do volume de frota pesada.
- **Qual hipótese será validada?**  
  A hipótese de que a concentração de sinistros com veículos pesados coincide com vazios assistenciais de Pontos de Parada e Descanso (distância > 50 km) e que a severidade/letalidade pode ser mapeada em corredores estratégicos para orientar investimentos públicos e de concessionárias.
- **Qual valor será entregue ao usuário final?**  
  Painéis interativos que permitem aos analistas do ONSV identificar rapidamente trechos com sinistros frequentes desprovidos de PPD, avaliar a taxa de severidade por frota tratora e visualizar a densidade de sinistros em rodovias federais e estaduais no Sudeste.

---

## 📝 Descrição da Solução

Desenvolvimento de uma interface de análise de dados e mapas temáticos em SVG/Web e relatórios estatísticos baseados no cruzamento de dados do Infosiga, PRF e registros de frota.

- **Funcionalidades principais incluídas:**
  * Mapa interativo de corredores rodoviários com cálculo de cobertura e identificação de trechos a mais de 50 km de um PPD credenciado/concessionado.
  * Mapeamento de pontos críticos (municípios com $\ge 30$ sinistros na janela e sem PPD em raio de 50 km).
  * Mapa de calor e densidade via KDE (Kernel Density Estimation) ao longo das rodovias do estado de São Paulo.
  * Módulo de correlação estatística entre o crescimento da frota registrada de caminhões/tratores e sinistros fatais (2015–2025).
  * Painel de densidade e distribuição de sinistros em rodovias federais (BRs) no Sudeste (SP, MG, RJ, ES).
- **Limitações conhecidas:**
  * As distâncias no MVP foram calculadas em linha reta (geodésica) a partir dos centroides municipais e marcos quilométricos dos PPDs, e não pelo traçado da malha rodoviária real (SNV/DNIT).
  * A frota refere-se ao município de emplacamento/registro do veículo, não refletindo o tráfego médio diário ponderado em cada trecho de via.
- **Escopo reduzido:**  
  Foco exclusivo em veículos de carga (pesados e caminhões-tratores) e passageiros nas principais rodovias estaduais paulistas e malha federal do Sudeste.

---

## 👥 Personas / Usuários-Alvo

- **Persona 1: Analista de Dados e Segurança Viária do ONSV**  
  * *Descrição:* Profissional responsável por conduzir estudos de acidentologia e formular propostas de segurança no trânsito.  
  * *Necessidades e Dores:* Necessita cruzar dados brutos de ocorrências (Infosiga/PRF) com a posição dos PPDs sem depender de processamentos manuais em planilhas isoladas; precisa de evidências estatísticas para embasar recomendações técnicas.
- **Persona 2: Gestor Público / Planejador de Logística de Transportes**  
  * *Descrição:* Tomador de decisão focado em infraestrutura logística rodoviária e concessões.  
  * *Necessidades e Dores:* Precisa de relatórios visuais e mapas de calor para priorizar a implantação de novos PPDs e dimensionar investimentos em trechos mais críticos e desassistidos.

---

## 🔑 User Stories (Backlog do MVP)

| ID | Prioridade | História de Usuário (User Story) | Estimativa | Sprint |
| :---: | :---: | :--- | :---: | :---: |
| **4** | Alta | **Como** analista do ONSV, **quero** calcular e mapear a distância entre os sinistros com veículos pesados e os Pontos de Parada e Descanso (PPD), **para que** eu identifique trechos desassistidos e padrões de risco por fadiga no estado de São Paulo. | 40 | 2 |
| **5** | Alta | **Como** analista do ONSV, **quero** analisar a correlação estatística entre o crescimento da frota pesada e o aumento de sinistros fatais em São Paulo, **para que** eu fundamente estudos de impacto logístico. | 40 | 2 |
| **6** | Média | **Como** analista do ONSV, **quero** visualizar a densidade de sinistros de veículos pesados no sudeste dentro das rodovias federais (BRs), **para que** eu localize visualmente os trechos rodoviários mais críticos e perigosos do estado. | 20 | 2 |

---

## 📅 Sprint(s) Relacionadas

| Sprint | Entregas Principais | Status |
| :---: | :--- | :---: |
| **01** | Coleta, auditoria, higienização das bases do Infosiga/PRF e estruturação do repositório analítico | Concluído |
| **02** | Mapas interativos (PPDs, KDE, Hotspots), cálculo de distâncias dos trechos críticos e correlação estatística frota × fatalidades | Concluído |

---

## 📊 Critérios de Aceitação

- O MVP deve permitir que o usuário filtre os mapas por corredor rodoviário (ex.: Anhanguera, Bandeirantes, Dutra, Régis Bittencourt, Castello Branco, Raposo Tavares) e visualize o raio de cobertura de cada PPD.
- O MVP deve permitir a consulta interativa dos municípios que compõem os "pontos críticos" (mínimo de 30 sinistros e PPD a mais de 50 km).
- O sistema deve registrar os índices de correlação linear ($r$) e p-valor das séries temporais (2015–2025) entre crescimento da frota de pesados e número de sinistros com vítimas fatais.
- Apresentar o ranking de sinistros por rodovia federal nas visualizações agregadas do Sudeste (BR-116, BR-381, BR-101, BR-040, etc.).
- Métricas coletadas na interface: tempo de resposta ao selecionar filtros e taxas de uso por camada analítica.

---

## 📈 Métricas de Validação

- **Número de usuários que testaram o MVP:** Validação com a equipe do projeto, orientador e analistas do ONSV.
- **Feedback qualitativo:** Avaliação da legibilidade visual dos mapas, clareza das legendas e consistência dos rankings de acidentalidade.
- **Indicadores de negócio:** Capacidade de quantificar com precisão o percentual de malha rodoviária desassistida (> 50 km de PPD) nos principais corredores de escoamento.

---

## 🚀 Próximos Passos

- Substituir as distâncias em linha reta pelo cálculo de roteirização sobre a malha viária real (SNV/DNIT).
- Refinar a precisão do mapa de calor (KDE) utilizando coordenadas georreferenciadas exatas de cada ocorrência.
- Ajustes de usabilidade e responsividade nos seletores da interface web.
- Expansão dos relatórios de correlação e densidade para outras regiões do país.
---

## 📂 Anexos / Evidências
- Prints de tela  
- Fluxos ou protótipos  
- Vídeo (MVP)  
