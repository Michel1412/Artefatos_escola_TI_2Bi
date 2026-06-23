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

```text
├── docs/
│   ├── index.html      # Página inicial — ponto de entrada da documentação
│   ├── requisitos/     # Histórias de usuário, casos de uso, regras de negócio
│   ├── diagramas/      # Arquitetura, diagramas de sequência e classes
│   ├── relatorios/     # Relatórios de atividades e sprints
│   ├── attachments/    # Imagens e arquivos referenciados pelas páginas HTML
│   └── styles/         # Estilos visuais exportados do Confluence
└── README.md           # Este arquivo de guia
```

---

## 📥 Como Acessar os Arquivos (após o `git clone`)

Este repositório contém documentação exportada do **Confluence** em formato HTML estático. Não é necessário instalar dependências nem subir servidor — basta clonar e abrir os arquivos no navegador.

### 1. Clonar o repositório

```bash
git clone https://github.com/Michel1412/Artefatos_escola_TI_2Bi.git
cd Artefatos_escola_TI_2Bi
```

### 2. Abrir a documentação no navegador

O ponto de entrada de toda a documentação é o arquivo **`docs/index.html`**.

**Windows (PowerShell):**
```powershell
Start-Process "docs\index.html"
```

**Linux / macOS:**
```bash
open docs/index.html        # macOS
xdg-open docs/index.html    # Linux
```

Também é possível abrir manualmente: navegue até a pasta `docs/` e dê duplo clique em `index.html`.

> **Importante:** Abra sempre pelo `index.html` ou pelos links internos das páginas. Os caminhos relativos entre pastas (`requisitos/`, `diagramas/`, `attachments/`) só funcionam corretamente quando a navegação parte de `docs/`.

### 3. Navegação entre as páginas

Cada página HTML possui:

- **Breadcrumb** (trilha no topo) — mostra a hierarquia e permite voltar às páginas-pai.
- **Link para o índice** — o primeiro item do breadcrumb sempre aponta para `index.html`.
- **Seção de anexos** — no final de cada página, lista os arquivos em `attachments/` (imagens, XML, etc.).

As imagens dos diagramas ficam em `docs/attachments/<id-da-pagina>/` e são carregadas automaticamente pelas páginas HTML.

---

## 🔍 Fluxo Recomendado para Análise

Para quem está avaliando o projeto pela primeira vez (professor, revisor ou novo integrante da equipe), siga esta ordem para entender o contexto completo do **LogViewer**:

### Etapa 1 — Visão geral do projeto
1. Leia este `README.md` para entender o propósito do sistema e os repositórios de código.
2. Abra **`docs/relatorios/32931841.html`** (*Relatório de Atividades*) — consolida o histórico de tarefas e o andamento geral no Jira.

### Etapa 2 — Requisitos e regras de negócio
Navegue a partir do índice (`docs/index.html`) até a seção de requisitos:

| Ordem | Arquivo                                             | Conteúdo                               |
|-------|-----------------------------------------------------|----------------------------------------|
| 1     | `docs/requisitos/Requisitos-de-Produto_950274.html` | Visão de produto e escopo              |
| 2     | `docs/requisitos/12091393.html`                     | Regras de negócio (versões por equipe) |
| 3     | `docs/requisitos/15761409.html`                     | Regras de negócio — versão final       |
| 4     | `docs/requisitos/Requisitos---Final_15663105.html`  | Documento consolidado de requisitos    |
| 5     | `docs/requisitos/99---Contexto-IA_15859713.html`    | Contexto da integração com IA          |

### Etapa 3 — Casos de uso (Sprint 3 em diante)
Os casos de uso estão organizados por sprint no índice. Comece por **`docs/relatorios/17498114.html`** (Sprint 3) e siga os links para cada caso numerado (CU-01 a CU-22), por exemplo:

- `docs/requisitos/21463041.html` — CU-01: Notificar Erros Encontrados
- `docs/requisitos/25264129.html` — CU-09: Interagir com Agente IA para Solução
- `docs/requisitos/27000833.html` — CU-21: Visualizar Dashboard Interativo

> Analise os casos de uso na ordem numérica para acompanhar a evolução funcional do sistema.

### Etapa 4 — Diagramas
Acesse a pasta **`docs/diagramas/`** ou use os links no índice, organizados por sprint:

| Sprint   | Relatório de referência         | Tipo de diagrama                        |
|----------|---------------------------------|-----------------------------------------|
| Sprint 4 | `docs/relatorios/25034769.html` | Diagramas de casos de uso (refatoração) |
| Sprint 5 | `docs/relatorios/38502401.html` | Diagramas de sequência (front-end)      |
| Sprint 6 | `docs/relatorios/49577989.html` | Diagramas de classe e DER               |

Diagramas principais:
- `docs/diagramas/Diagrama-de-Classe-Geral_64061441.html` — modelo de classes geral
- `docs/diagramas/Diagrama-de-Classe-1_54198302.html` — diagrama de classes (versão 1)

### Etapa 5 — Relatórios de sprint (cronologia)
Para acompanhar a evolução do projeto ao longo do semestre, leia os relatórios na ordem cronológica:

1. `docs/relatorios/1441956.html` — Atividade 3: Construção de ideias
2. `docs/relatorios/Sprint-2---Atividade-4_4718593.html` — Sprint 2
3. `docs/relatorios/17498114.html` — Sprint 3
4. `docs/relatorios/25034769.html` — Sprint 4
5. `docs/relatorios/38502401.html` — Sprint 5
6. `docs/relatorios/49577989.html` — Sprint 6
7. `docs/relatorios/67108866.html` — Sprint 6: Modelagem de Dados (DER)

### Etapa 6 — Código-fonte (repositórios externos)
Após compreender os artefatos de documentação, consulte a implementação nos repositórios listados na seção [Repositórios do Ecossistema](#-repositórios-do-ecossistema).

---

### Resumo visual do fluxo

```text
git clone
    │
    ▼
docs/index.html  ──────────────────────────────────────────┐
    │                                                       │
    ├── README.md (visão geral)                             │
    ├── relatorios/32931841.html (relatório geral)          │
    ├── requisitos/ (produto → regras → casos de uso)       │
    ├── diagramas/ (sequência → classes → DER)              │
    ├── relatorios/ (sprints em ordem cronológica)          │
    └── repositórios GitHub (front-end e back-end)  ◄───────┘
```