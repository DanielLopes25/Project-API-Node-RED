# 📡 Project API Node-RED — BrazilAPI Integration

Este projeto foi desenvolvido como parte de um desafio, utilizando **Node-RED** para criar um aplicativo web capaz de consultar APIs públicas do serviço **BrazilAPI**  
🔗 https://brasilapi.com.br/

A aplicação possui duas funcionalidades:

- 🏦 **Consulta das Corretoras Ativas da CVM**, com lista filtrável  
- 📮 **Busca de CEP (CEP v2)** exibindo Rua, Bairro, Cidade/UF, Latitude e Longitude  

O objetivo foi demonstrar conhecimento em integrações REST, desenvolvimento visual com Node-RED e construção de interfaces HTML com Bootstrap.

---

# 🚀 Começando

Estas instruções permitirão que você configure e execute o projeto na sua máquina local para fins de desenvolvimento, testes e avaliação.

---

# 📋 Pré-requisitos

Para rodar o projeto, você precisa ter instalado:

- **Node.js** (versão 14+)
- **Node-RED**  
  Instalação:
  ```bash
  npm install -g node-red
- Navegador web (Chrome, Edge, Firefox, etc.)

- 🔧 Instalação

Siga estas etapas para configurar o ambiente:

1️⃣ Clone o repositório
git clone https://github.com/DanielLopes25/Project-API-Node-RED

2️⃣ Acesse o diretório do projeto
cd Project-API-Node-RED>

3️⃣ Inicie o Node-RED
node-red

4️⃣ Abra no navegador
http://localhost:1880

5️⃣ Importe os fluxos

Menu (☰) → Import

Selecione o arquivo flows.json

Clique em Import

Clique em Deploy



⚙️ Executando os testes

Este projeto não possui testes automatizados formais por ser um desafio técnico focado em integração API + Node-RED.
Entretanto, recomenda-se testar manualmente:

✔ Teste do Broker Catalog

Rota:

http://localhost:1880/brokers


Verificar:

Carregamento das corretoras

Filtro funcionando

Botão para acessar o ZIP Code Searcher

✔ Teste do Zip Code Searcher (Formulário)
http://localhost:1880/cep-form


Digite:

89010025


Verificar se os dados carregam corretamente.

