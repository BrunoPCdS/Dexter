<div align="center">

# 🤖 Dexter — Assistente Pessoal Inteligente com IA

**Gerenciamento inteligente de rotinas e tarefas por comando de voz, texto e quadro Kanban.**

[![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactnative.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![PostgreSQL](https://img.shields.io/badge/Neon_Postgres-316192?style=for-the-badge&logo=postgresql&logoColor=white)](https://neon.tech/)
[![Groq](https://img.shields.io/badge/Groq-000000?style=for-the-badge)](https://groq.com/)
[![ElevenLabs](https://img.shields.io/badge/ElevenLabs-000000?style=for-the-badge)](https://elevenlabs.io/)
[![UML](https://img.shields.io/badge/PlantUML-000000?style=for-the-badge&logo=uml&logoColor=white)](https://plantuml.com/)

> Repositório oficial da disciplina de **Projeto de Desenvolvimento 1** — *Análise e Desenvolvimento de Sistemas*.

</div>

---

## 🖼️ Telas da Aplicação

<p align="center">
  <img src="./imgs/img%20(1).jpg" alt="Tela da aplicação 1" width="220">
  <img src="./imgs/img%20(2).jpg" alt="Tela da aplicação 2" width="220">
  <img src="./imgs/img%20(3).jpg" alt="Tela da aplicação 3" width="220">
  <img src="./imgs/img%20(4).jpg" alt="Tela da aplicação 4" width="220">
</p>
<p align="center">
  <img src="./imgs/img%20(5).jpg" alt="Tela da aplicação 5" width="220">
  <img src="./imgs/img%20(6).jpg" alt="Tela da aplicação 6" width="220">
  <img src="./imgs/img%20(7).jpg" alt="Tela da aplicação 7" width="220">
  <img src="./imgs/img%20(8).jpg" alt="Tela da aplicação 8" width="220">
</p>

## 📖 Visão Geral

O **Dexter** é uma aplicação mobile assistiva voltada à produtividade e administração pessoal. Através de **Transcrição de Áudio (Speech-to-Text)** e **Processamento de Linguagem Natural**, o sistema atua como um copiloto diário: o usuário pode enviar um áudio ou digitar para cadastrar suas tarefas, organizar seu fluxo de trabalho em um quadro **Kanban** interativo e receber um retorno imediato com dicas práticas geradas por Inteligência Artificial sobre como executar cada atividade com mais eficiência.

---

## ✨ Funcionalidades e Escopo do Sistema

### 👤 Gestão de Conta e Autenticação
- Cadastro, autenticação segura e gerenciamento de perfil do usuário.

### 📋 Gestão Inteligente de Tarefas (Kanban & IA)
- **Entrada por Voz (Transcrição) ou Texto:** O usuário envia um áudio falando sua pendência; o sistema transcreve automaticamente o conteúdo e estrutura a tarefa (ou permite o cadastro manual via texto).
- **Retorno de Dicas de Execução via IA:** A partir da tarefa criada ou selecionada, a IA analisa o contexto e retorna dicas práticas e passos acionáveis para auxiliar na sua conclusão.
- **Quadro Kanban Interativo:** Organização visual e movimentação das tarefas por status (*A Fazer*, *Em Andamento*, *Concluído*).
- **Edição e Exclusão:** Controle completo sobre prazos, títulos, descrições e prioridades.

---

## 📐 Arquitetura e Modelagem UML

O projeto conta com documentação técnica baseada nos padrões da **UML**, utilizando **PlantUML / Astah** para mapear os requisitos e interações do sistema:

- **Atores Principais:**
  - **Usuário:** Interage com o aplicativo enviando áudios/textos, gerenciando sua conta, movimentando o quadro Kanban e consultando as dicas da IA.
- **Sistemas Externos / Atores Secundários:**
  - **API de IA (Groq):** Responsável pela transcrição do áudio enviado pelo usuário (Speech-to-Text) utilizando o modelo Whisper.
  - **API de voz (ElevenLabs):** Responsável pela comunicação conversacional do agente de voz.
- **Artefatos no Repositório:** Os diagramas de Casos de Uso (`.puml` / imagens exportadas) e especificações técnicas encontram-se organizados nos diretórios de documentação do projeto.

---

## 🛠️ Stack Tecnológica

| Camada | Tecnologias Utilizadas |
| :--- | :--- |
| **Front-end (Mobile)** | React Native, Expo, TypeScript, Expo Audio, Expo Secure Store |
| **Back-end** | Node.js, Express, TypeScript, REST API, JWT, Zod |
| **Banco de Dados** | PostgreSQL (Neon), Prisma ORM |
| **Inteligência Artificial** | Groq API (Whisper para transcrição de áudio), ElevenLabs (agente conversacional) |
| **Documentação & Modelagem** | Markdown, diagramas UML |
| **Controle de Versão** | Git & GitHub |

---

## 👥 Equipe de Desenvolvimento

| Integrante | Função / Papel no Projeto | Responsabilidades Principais |
| :--- | :--- | :--- |
| [**Dione**](https://github.com/Dione6030) | Product Owner (PO) | Visão do produto, levantamento de requisitos e gestão de backlog. |
| [**Bruno**](https://github.com/BrunoPCdS) | Desenvolvedor full stack | Desenvolvimento mobile em React Native, captura de áudio, telas do Kanban, UI/UX ajustes backend |
| [**Ítalo**](https://github.com/istalo) | Desenvolvedor Back-end | Arquitetura da API em Node.js/TypeScript, banco de dados Neon e integração de transcrição/IA. |
| [**Lucas**](https://github.com/lucasrochaexe) | Documentador Técnico / Arquitetura | Modelagem de sistemas, diagramas UML e documentação técnica do repositório. |

---

## 📂 Estrutura de Diretórios

```plaintext
Projeto-de-Desenvolvimento-1/
├── back/                       # API Node.js/TypeScript, rotas, banco e integrações de IA
├── front/                      # Aplicação cliente desenvolvida em React Native e Expo
├── docs/                       # Documentação técnica e diagramas
├── imgs/                       # Imagens das telas da aplicação
└── README.md                   # Documentação principal do projeto

📊 Status do Projeto (Roadmap)
[x] Definição do escopo do produto e papéis da equipe

[x] Modelagem e refinamento do Diagrama de Casos de Uso em PlantUML

[x] Estruturação do banco de dados em nuvem (Neon Postgres)

[x] Implementação do fluxo de envio de áudio, transcrição e geração de dicas com IA

[x] Construção do fluxo principal e quadro Kanban no React Native

[X] Testes integrados de ponta a ponta (Front-end ↔ Back-end ↔ IA)

[ ] Apresentação e entrega final da disciplina
