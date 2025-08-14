# Sistema de Credenciamento e Business Intelligence para Eventos

![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white) ![AppSheet](https://img.shields.io/badge/AppSheet-2173E3?style=for-the-badge&logo=appsheet&logoColor=white) ![Looker Studio](https://img.shields.io/badge/Looker_Studio-4285F4?style=for-the-badge&logo=looker-studio&logoColor=white) ![Tally](https://img.shields.io/badge/Tally-000000?style=for-the-badge&logo=tally&logoColor=white)

Um case de estudo sobre a construção de um ecossistema completo para gestão de credenciamento, check-in e análise de dados em tempo real para o evento "A Jornada do Consumidor", utilizando ferramentas low-code e no-code para máxima eficiência e mínimo custo.

---

### Tabela de Conteúdos
1. [Visão Geral do Projeto](#1-visão-geral-do-projeto)
2. [O Desafio](#2-o-desafio)
3. [A Solução Proposta (O Ecossistema)](#3-a-solução-proposta-o-ecossistema)
4. [Tecnologias Utilizadas](#4-tecnologias-utilizadas)
5. [Funcionalidades em Destaque](#5-funcionalidades-em-destaque)
6. [Resultados e Valor Agregado](#6-resultados-e-valor-agregado)

---

### 1. Visão Geral do Projeto
Este projeto documenta a criação de um sistema robusto para gerenciar o credenciamento de um evento local para 500 pessoas. A solução abrange desde a inscrição inteligente do participante até a análise de dados pós-evento, utilizando um ecossistema de ferramentas gratuitas e integradas para criar uma experiência profissional e gerar inteligência de negócio.

### 2. O Desafio
O objetivo era criar um sistema de credenciamento para o evento "A Jornada do Consumidor - 2ª Edição" com as seguintes características:
- **Público:** 500 participantes, divididos em dois turnos com perfis diferentes (vendedores/operacional e empresários).
- **Funcionalidades:** Formulário com lógica condicional, geração de QR Code único, check-in rápido via app, crachás personalizados e um dashboard para a organização.
- **Restrições:** Custo de software próximo de zero, alta confiabilidade e uma experiência fluida para o participante e para a equipe de credenciamento.

### 3. A Solução Proposta (O Ecossistema)
Para resolver o desafio, foi projetada uma arquitetura de dados centralizada no Google Workspace, onde cada ferramenta desempenha um papel específico, mas integrado, garantindo um fluxo de dados perfeito e em tempo real.

**Diagrama da Arquitetura:**
![Diagrama da Arquitetura](./assets/diagrama-arquitetura.png)

### 4. Tecnologias Utilizadas
- **Tally.so:** Utilizado para a criação do formulário de inscrição inteligente, com lógica condicional para adaptar as perguntas ao perfil do participante.
- **Google Sheets:** O "cérebro" da operação, servindo como banco de dados central. Fórmulas foram usadas para categorizar participantes e gerar links de QR Code dinamicamente.
- **Google AppSheet:** Usado para criar um aplicativo de check-in personalizado para a equipe do evento, permitindo a validação de participantes via QR Code de forma instantânea e profissional.
- **Google Looker Studio:** Para a criação de um dashboard em tempo real, exibindo métricas como total de inscritos, taxa de comparecimento (show-up rate) e perfil do público presente.
- **Canva:** Utilizado para o design dos crachás, com a função "Criação em Lote" para personalização em massa a partir dos dados da planilha.

### 5. Funcionalidades em Destaque

**App de Check-in Personalizado em Ação:**
*Para garantir um check-in rápido e sem erros, foi desenvolvido um aplicativo interno com o Google AppSheet. A equipe de credenciamento utiliza o app para escanear o QR Code do participante, o que filtra instantaneamente a lista de inscritos. Com um único toque, o check-in é confirmado e a base de dados é atualizada em tempo real. Veja em funcionamento:*
![Check-in em Ação](./assets/gif-app-checkin.gif)

**Dashboard em Tempo Real:**
*Um painel de comando foi criado no Google Looker Studio para a organização do evento. O dashboard mostra ao vivo os principais KPIs: total de presentes, taxa de comparecimento, o perfil do público que já chegou (separado por tipo de acesso) e o fluxo de entradas ao longo do dia, transformando dados operacionais em inteligência de negócio.*
![Dashboard de Comando](./assets/screenshot-dashboard.jpg)

### 6. Resultados e Valor Agregado
A implementação deste sistema entregou valor em múltiplas frentes:
- **Experiência Profissional:** Os participantes receberam uma comunicação clara e tiveram um check-in rápido e tecnológico, com tempo médio inferior a 15 segundos por pessoa.
- **Eficiência Operacional:** A equipe de credenciamento operou com uma ferramenta customizada, eliminando filas e erros manuais.
- **Inteligência de Dados:** A contratante teve acesso a um dashboard com métricas em tempo real, permitindo uma visão clara do andamento do evento e do perfil do público.
- **Custo Zero de Software:** Todo o sistema foi construído com planos gratuitos das ferramentas, provando que é possível entregar uma solução de alto nível com criatividade e estratégia.
