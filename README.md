# 📡 Project API Node-RED — BrazilAPI Integration
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Node-RED](https://img.shields.io/badge/Node--RED-API%20Flows-red)
![BrazilAPI](https://img.shields.io/badge/BrazilAPI-v2-blue)

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

### ✔ Broker Catalog  
![Broker Catalog](https://github.com/DanielLopes25/Project-API-Node-RED/blob/main/Picture%20Broker%20Catalog.png)

### ✔ Resultado de CEP  
![CEP Result](https://github.com/DanielLopes25/Project-API-Node-RED/blob/main/CEP%20Result.png)

### ✔ Flow Node-RED 
![Flow node-RED](https://github.com/DanielLopes25/Project-API-Node-RED/blob/main/Picture%20Flow%20Node%20RED.png)




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
git clone https://github.com/DanielLopes25/Project-API-Node-RED


2️⃣ Acesse o projeto
bash
cd <Project-API-Node-RED>


3️⃣ Inicie o Node-RED
bash
node-red


4️⃣ Acesse no navegador
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

