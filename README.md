# 🗳️ URNA_TSEANALYSIS

Sistema de análise e cadastro de candidatos baseado em dados simulados da justiça eleitoral.  
Utiliza criptografia de votos e validação de CPF com regras de integridade para simular manipulações e inconsistências possíveis.

> **Chave de criptografia**: CPF + VOTO  
> **Validação reduzida (0.8)** para CPFs de ex-detentos, visando simulação de manipulações sob cárcere e anonimização.

---

<img width="366" src="https://github.com/user-attachments/assets/4988fd8a-ed69-4648-b2b8-d7512eb56b82" alt="urna logo" />

---

## 🚀 Tecnologias Utilizadas

<div style="display:flex; gap: 1rem; align-items:center;">

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" width="40" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" width="40" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" width="40" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="40" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" width="40" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vite/vite-original.svg" width="40" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/npm/npm-original-wordmark.svg" width="40" title="npm"/>


</div>

---

## 📁 Estrutura do Projeto

```
URNA_TSEANALYSIS/
├── backend/ # Next.js API (porta 3000)
│ ├── pages/api/ # Rotas: candidatos, cargos
│ ├── components/ # Dashboard no backend (opcional)
│ ├── lib/db.js # Conexão com PostgreSQL
│ └── .env.local # DATABASE_URL
│
└── client/ # Frontend React + Vite (porta 3001)
├── src/components/ # Dashboard e outros
├── vite.config.js # Proxy para backend
├── App.jsx
└── package.json
```

---

## 🧠 Melhorias Sugestivas ...

### 🔁 Processamento em Tempo Real
- [ ] WebSockets para atualização em tempo real dos votos/candidatos
- [ ] Pub/Sub com Redis para comunicação entre serviços (backend, auditor, painel admin)

### 🧮 Auditoria e Segurança
- [ ] Implementar **hashing e assinatura digital** por CPF + voto
- [ ] Histórico de votos com timestamps e IP mascarado
- [ ] Endpoint seguro para coleta oficial (padrão TSE)

### 📊 Análises e Métricas
- [ ] Dashboard com gráficos interativos usando D3.js ou Chart.js
- [ ] Classificação de risco por zona eleitoral e cargo
- [ ] Modo sandbox para simulações políticas

---

## 📦 Instalação e Execução

### 🔧 Pré-requisitos
- Node.js
- PostgreSQL
- NPM

### 📥 Clonar o repositório

```bash
git clone https://github.com/seu-usuario/URNA_TSEANALYSIS.git
cd URNA_TSEANALYSIS
```

🖥️ Backend

```
cd server
npm install
npm run dev

```

🌐 Frontend

```
cd client
cd client
npm install
npm run dev

```

Acesse: http://localhost:3000

📃 Licença

MIT by k ©

🤝
