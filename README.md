# Governança Mínima Viável (GMV) - Painel Preventivo CISE

Este repositório contém a documentação e os artefatos do projeto de **Governança Mínima Viável (GMV)** para o Centro Integrado de Serviços Essenciais (CISE). [cite_start]O objetivo é estabelecer uma "Unidade de Comando Informativa" para prevenir falhas em serviços críticos do Estado[cite: 87, 89].

## Visão Geral do Projeto
[cite_start]O CISE foi criado para integrar dados de secretarias que hoje operam em silos, eliminando definições métricas conflitantes e garantindo um "número oficial" para a tomada de decisão do Governador[cite: 4, 6, 92].

* [cite_start]**Foco:** Agilidade preventiva vs. contagem reativa[cite: 113].
* [cite_start]**Prazo do Piloto:** 60 dias[cite: 175].
* [cite_start]**Público-alvo:** Governador e Secretários de Estado[cite: 125, 174].

---

## 1. Escopo do Piloto (KPIs Oficiais)
[cite_start]O painel monitora 5 indicadores preventivos com atualização **semanal** e recorte territorial por **bairro**[cite: 22, 23]:

1.  [cite_start]**Saneamento:** Disponibilidade da rede (Pressão/Vazão)[cite: 100].
2.  [cite_start]**Energia Crítica:** Estabilidade elétrica (Autonomia de geradores em hospitais)[cite: 101, 102].
3.  [cite_start]**Defesa Civil:** Índice de Vulnerabilidade de Encostas (Saturação do solo)[cite: 103, 104].
4.  [cite_start]**Mobilidade:** Fluidez de emergência (Tempo de resposta em vias arteriais)[cite: 106, 107].
5.  [cite_start]**Saúde:** Prontidão de insumos (Estoque de medicamentos críticos e oxigênio)[cite: 109, 110].

> [cite_start]**Fora do Escopo:** Prontuários individuais e dados nominais, visando a minimização de riscos de privacidade[cite: 114].

---

## 2. Matriz de Responsabilidade (RACI)
[cite_start]A governança equilibra a autonomia das secretarias com a padronização centralizada do CISE[cite: 127, 129]:

| Atividade | Data Owner (Secretário) | Data Steward (Técnico) | Custodiante (TI CISE) |
| :--- | :---: | :---: | :---: |
| Definir KPI Oficial | **Aprova** | **Responsável** | Consultado |
| Tratar Conflitos | **Aprova** | **Responsável** | Informado |
| Publicar no Painel | Informado | Consultado | **Responsável** |
| Aprovar Microdados | **Aprova** | **Responsável** | Informado |

[cite_start][cite: 128]

---

## 3. Políticas de Governança
[cite_start]Para garantir a sustentabilidade do projeto, aplicam-se três regras fundamentais[cite: 131]:

* [cite_start]**Single Source of Truth (SSOT):** O dado do CISE é o único valor oficial reconhecido; divergências são tratadas como incidentes[cite: 132, 134].
* **Minimização de Acesso:** O acesso padrão é ao dado agregado. [cite_start]Microdados exigem justificativa formal e aprovação do Owner[cite: 135, 137].
* [cite_start]**Versionamento de Regras:** Mudanças no cálculo de um KPI exigem 15 dias de antecedência e comunicação de impacto[cite: 138, 139].

---

## 4. Checklist de Qualidade (Semáforo)
[cite_start]Nenhum dado é publicado sem passar pelo crivo de qualidade mínima[cite: 53, 142]:

1.  [cite_start]**Completude:** Mínimo de 98% de cobertura territorial[cite: 149].
2.  [cite_start]**Consistência Temporal:** Dados estritamente da semana vigente[cite: 151].
3.  [cite_start]**Integridade Territorial:** Eventos obrigatoriamente vinculados a bairros válidos[cite: 153].

[cite_start]**Se o checklist falhar:** O painel recebe uma **Tarja Amarela** (Alerta de Confiança) e abre-se um SLA de 48h para correção na fonte[cite: 155, 156].

---

## 5. Roadmap 90 Dias
* [cite_start]**30 Dias:** Homologação do Glossário e RACI[cite: 172, 174].
* [cite_start]**60 Dias:** Lançamento oficial com carga automática via APIs[cite: 175, 176].
* [cite_start]**90 Dias:** Implementação do Catálogo de Metadados e automação completa[cite: 178, 179].
