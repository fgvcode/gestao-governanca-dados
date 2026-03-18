# Governança Mínima Viável (GMV) - Painel Preventivo CISE

Este repositório contém a documentação e os artefatos do projeto de **Governança Mínima Viável (GMV)** para o Centro Integrado de Serviços Essenciais (CISE). [cite_start]O objetivo é estabelecer uma "Unidade de Comando Informativa" para prevenir falhas em serviços críticos do Estado.

## Visão Geral do Projeto
O CISE foi criado para integrar dados de secretarias que hoje operam em silos, eliminando definições métricas conflitantes e garantindo um "número oficial" para a tomada de decisão do Governador.

* **Foco:** Agilidade preventiva vs. contagem reativa.
* **Prazo do Piloto:** 60 dias.
* **Público-alvo:** Governador e Secretários de Estado.

---

## 1. Escopo do Piloto (KPIs Oficiais)
O painel monitora 5 indicadores preventivos com atualização **semanal** e recorte territorial por **bairro**:

1.  **Saneamento:** Disponibilidade da rede (Pressão/Vazão)[cite: 100].
2.  **Energia Crítica:** Estabilidade elétrica (Autonomia de geradores em hospitais).
3.  **Defesa Civil:** Índice de Vulnerabilidade de Encostas (Saturação do solo).
4.  **Mobilidade:** Fluidez de emergência (Tempo de resposta em vias arteriais).
5.  **Saúde:** Prontidão de insumos (Estoque de medicamentos críticos e oxigênio).

>**Fora do Escopo:** Prontuários individuais e dados nominais, visando a minimização de riscos de privacidade.

---

## 2. Matriz de Responsabilidade (RACI)
[cite_start]A governança equilibra a autonomia das secretarias com a padronização centralizada do CISE:

| Atividade | Data Owner (Secretário) | Data Steward (Técnico) | Custodiante (TI CISE) |
| :--- | :---: | :---: | :---: |
| Definir KPI Oficial | **Aprova** | **Responsável** | Consultado |
| Tratar Conflitos | **Aprova** | **Responsável** | Informado |
| Publicar no Painel | Informado | Consultado | **Responsável** |
| Aprovar Microdados | **Aprova** | **Responsável** | Informado |


---

## 3. Políticas de Governança
Para garantir a sustentabilidade do projeto, aplicam-se três regras fundamentais:

* **Single Source of Truth (SSOT):** O dado do CISE é o único valor oficial reconhecido; divergências são tratadas como incidentes.
* **Minimização de Acesso:** O acesso padrão é ao dado agregado. [cite_start]Microdados exigem justificativa formal e aprovação do Owner.
* **Versionamento de Regras:** Mudanças no cálculo de um KPI exigem 15 dias de antecedência e comunicação de impacto.

---

## 4. Checklist de Qualidade (Semáforo)
Nenhum dado é publicado sem passar pelo crivo de qualidade mínima:

1. **Completude:** Mínimo de 98% de cobertura territorial.
2. **Consistência Temporal:** Dados estritamente da semana vigente.
3. **Integridade Territorial:** Eventos obrigatoriamente vinculados a bairros válidos.

[cite_start]**Se o checklist falhar:** O painel recebe uma **Tarja Amarela** (Alerta de Confiança) e abre-se um SLA de 48h para correção na fonte.

---

## 5. Roadmap 90 Dias
* **30 Dias:** Homologação do Glossário e RACI.
* **60 Dias:** Lançamento oficial com carga automática via APIs.
* **90 Dias:** Implementação do Catálogo de Metadados e automação completa.
