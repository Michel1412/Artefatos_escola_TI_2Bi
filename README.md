# Artefatos do Projeto - LogViewer 🪵🔍

Este repositório centraliza toda a documentação, diagramas e artefatos de gerenciamento do projeto **LogViewer**, desenvolvido para a disciplina **Escola de TI**, ministrada pelo **Professor João Choma**.

---

## 👥 Equipe

* Michel Bocchi Junior - 232207803-2
* Felipe Barreto Cortes -  23069437-2
* João Pedro Souza Peixoto Saraiva - 23024350-2
* Pedro Alvaro Mantuani Silva - 23079477-2
* ⁠André Felipe Ferrari de Azevedo - 22120196-2
* Vinicius Reginaldo Ferrarini - 23159293-2

---

## 🚀 Sobre o Projeto LogViewer

O **LogViewer** é uma solução robusta e inteligente para a gestão de logs corporativos. Ele foi projetado para ir muito além de um simples visualizador de arquivos, oferecendo uma infraestrutura completa de monitoramento e resposta a incidentes.

### Como funciona:
1. **Coleta Eficiente:** Através de um **SDK integrado**, o sistema gerencia e envia os logs da aplicação do cliente em pacotes para o nosso backend.
2. **Análise e Detecção:** O backend processa os dados e identifica falhas críticos ou anomalias em tempo real.
3. **Notificação Instantânea:** O cliente é alertado imediatamente na palma da mão via **notificações push no celular** e através de alertas visuais em um **dashboard web**.
4. **Inteligência Artificial:** O projeto se estende com a integração de uma **LLM (Large Language Model)**, que analisa o erro encontrado e sugere automaticamente uma solução para o problema.

---

## 📋 Artefatos de Gerenciamento e Documentação

Os artefatos contidos neste repositório refletem o planejamento e a execução do projeto nas plataformas de gestão:

*   **Gestão de Tarefas (Jira):** [Painel de Controle e Histórias de Usuário](https://groupfromthesouth.atlassian.net/jira/software/projects/TR/summary?atlOrigin=eyJpIjoiNmNkZTJlMzdhMTYzNGZmNmE0Y2ZkODQ4NWNkMGUyZjYiLCJwIjoiaiJ9)
*   **Documentação Técnica (Confluence):** [Relatório de Atividades do Projeto](https://groupfromthesouth.atlassian.net/wiki/spaces/TR/pages/32931841/Relat+rio+de+Atividades)

---

## 💻 Repositórios do Ecossistema

O desenvolvimento do código-fonte do sistema está dividido nos seguintes repositórios:

*   🖥️ **Front-end (Dashboard Web):** [GitHub - LogView Front-end](https://github.com/OImmortal/LogView)
*   ⚙️ **Back-end (API, SDK & Integração LLM):** [GitHub - LogViewer Back-end](https://github.com/OImmortal/logview-backend)

---

## 🗂️ Estrutura deste Repositório

*(Dica: Caso você organize os arquivos em pastas dentro deste repositório, você pode listá-los aqui de forma organizada)*

```text
├── /requisitos        # Histórias de usuário exportadas, BDDs ou PDFs do Jira
├── /diagramas          # Arquitetura do sistema, diagramas de sequência do SDK
├── /relatorios         # Cópias ou complementos do Relatório de Atividades
└── README.md           # Este arquivo de guia
