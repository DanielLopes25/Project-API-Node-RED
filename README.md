# 📡 Project API Node-RED — BrazilAPI Integration
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Node-RED](https://img.shields.io/badge/Node--RED-API%20Flows-red)
![BrazilAPI](https://img.shields.io/badge/BrazilAPI-v2-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

Aplicação desenvolvida como **desafio**, utilizando **Node-RED** para integração com a **BrazilAPI**, criando um mini-sistema web com duas funcionalidades principais:

- 🏦 **Broker Catalog** — Lista todas as corretoras ativas registradas na CVM  
- 📮 **Zip Code Searcher (CEP v2)** — Consulta e exibe dados completos de um CEP  

O projeto demonstra o uso de APIs REST, desenvolvimento orientado a fluxos, templates HTML com Bootstrap e integração entre diferentes rotas HTTP no Node-RED.

---

# 🚀 Funcionalidades

## 🏦 Broker Catalog
Consulta automática à API:

https://brasilapi.com.br/api/cvm/corretoras/v1


Funcionalidades:
- Lista todas as corretoras ativas da CVM  
- Interface clara e moderna (Bootstrap)  
- 🔍 Filtro em tempo real por nome, cidade ou CNPJ  
- Navegação integrada com o Zip Code Searcher  

---

## 📮 Zip Code Searcher — CEP 
Consulta à API:

https://brasilapi.com.br/api/cep/v2/{cep}


Retorna:
- Rua  
- Bairro  
- Cidade / UF  
- Botões de navegação entre páginas

Modos de uso:

| Tipo | Rota | Exemplo |
|------|------|---------|
| Via formulário | `/cep-form` | formulário elegante com Bootstrap |
| Via querystring | `/cep-lookup?cep=89010025` | input rápido |

---

# 🖼 Screenshots  
*(adicione as imagens reais depois na pasta `/screenshots`)*

### ✔ Broker Catalog  
![Broker Catalog](screenshots/brokers.png)

### ✔ Formulário de CEP  
![CEP Form](screenshots/cep-form.png)

### ✔ Resultado do CEP  
![CEP Result](screenshots/cep-result.png)

---

# 📂 Estrutura do Repositório

node-red-brazilapi-challenge/
│
├── flows.json # Fluxos exportados do Node-RED
├── README.md # Documentação completa
└── screenshots/ # Imagens do projeto (opcional)



---

# 📋 Pré-requisitos

Para rodar o projeto, instale:

- **Node.js (LTS recomendado)**  
- **Node-RED**  
  ```bash
  npm install -g node-red
Um navegador moderno (Chrome, Edge, Firefox…)

🔧 Instalação
1️⃣ Clone o repositório
bash
Copiar código
git clone https://github.com/<seu-usuario>/<nome-repositorio>.git
2️⃣ Acesse o projeto
bash
Copiar código
cd <nome-repositorio>
3️⃣ Inicie o Node-RED
bash
Copiar código
node-red
4️⃣ Acesse no navegador
arduino
Copiar código
http://localhost:1880
📥 Importando os Fluxos
Acesse o Node-RED

Menu superior ☰ → Import

Selecione o arquivo flows.json

Clique em Import

Clique em Deploy

Pronto! 🚀

🧭 Rotas da Aplicação
📌 Broker Catalog
Método	Rota	Descrição
GET	/brokers	Lista corretoras da CVM com busca em tempo real

📌 Zip Code Searcher
Método	Rota	Descrição
GET	/cep-form	Formulário de busca de CEP
GET	/cep-lookup	Busca CEP via querystring
GET	/cep/:cep	Busca CEP via parâmetro de rota

⚙️ Testes Manuais (Recomendados)
✔ Broker Catalog
bash
Copiar código
http://localhost:1880/brokers
Verificar se lista carrega

Testar filtro

Testar navegação

✔ CEP via formulário
bash
Copiar código
http://localhost:1880/cep-form


✒️ Autor
Daniel de Sales Lopes
📍 Betim — MG
📧 danieldesales.mct@gmail.com
🔗 https://www.linkedin.com/in/danielsaleslopes/

