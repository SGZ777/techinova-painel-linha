# 🚀 TechInova - Painel Linha

> **Painel de Monitoramento e Gestão em Tempo Real para Linhas de Produção e Operações.**

![Release](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Status](https://img.shields.io/badge/status-ativo-brightgreen.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

---

## 📌 Sobre o Projeto

O **TechInova Painel Linha** é uma solução desenvolvida para a visualização, acompanhamento e telemetria em tempo real do desempenho de linhas operacionais e de produção. 

Projetado para ambientes industriais e corporativos, a plataforma consolida métricas essenciais como eficiência global (OEE), tempo de ciclo, contagem de produção, parada de máquinas e alertas operacionais em uma interface limpa, intuitiva e otimizada para displays/dashboards de chão de fábrica.

---

## ✨ Principais Funcionalidades

- ⏱️ **Monitoramento em Tempo Real:** Atualização contínua do status da linha de produção via WebSockets/MQTT.
- 📊 **Indicadores de Desempenho (KPIs):**
  - OEE (Overall Equipment Effectiveness / Eficiência Global).
  - Taxa de Qualidade, Disponibilidade e Performance.
  - Metas vs. Produção Realizada.
- 🚨 **Gestão de Alertas e Incidentes:** Notificação visual de interrupções, paradas de linha (Andon) e solicitações de manutenção.
- 🖥️ **Modo TV / Kiosk:** Interface adaptada para exibição em monitores industriais e TVs sem necessidade de interação constante.
- 📈 **Histórico e Relatórios:** Registro detalhado de eventos e paradas para auditoria e análise preditiva.
- 🔐 **Controle de Acesso (RBAC):** Níveis de permissão diferenciados para operadores, supervisores e administradores.

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído utilizando as seguintes tecnologias:

### Frontend
- **Framework:** [React.js](https://reactjs.org/) / [Next.js](https://nextjs.org/)
- **Estilização:** Tailwind CSS / Styled Components
- **Gráficos & Visualização:** Chart.js / Recharts
- **Comunicação em Tempo Real:** Socket.io-client / MQTT.js

### Backend & Integração
- **Runtime:** Node.js / Python (FastAPI/Flask)
- **Banco de Dados:** PostgreSQL / MongoDB / Redis (Cache de métricas instantâneas)
- **Mensageria:** RabbitMQ / Mosquitto MQTT Broker

---

## 📁 Estrutura do Projeto

```text
techinova-painel-linha/
├── public/              # Arquivos estáticos e ativos de imagem
├── src/
│   ├── assets/          # Ícones, estilos globais e temas
│   ├── components/      # Componentes reutilizáveis de UI (KpiCard, Chart, AlertBanner)
│   ├── config/          # Configurações de API e ambiente
│   ├── hooks/           # Custom React Hooks (ex: useWebSocket, useProductionData)
│   ├── pages/           # Rotas e visões da aplicação
│   ├── services/        # Integração de API, Socket e repositórios de dados
│   ├── types/           # Interfaces e definições de tipos TypeScript
│   └── utils/           # Funções utilitárias e formatadores de dados
├── .env.example         # Modelo de variáveis de ambiente
├── docker-compose.yml   # Containerização da aplicação
├── package.json         # Dependências do projeto
└── README.md            # Documentação principal
