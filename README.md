👤 Cadastro de Usuários — React App

Aplicação front-end desenvolvida em React para cadastro e navegação de usuários, integrada a uma API REST.
O projeto foi criado com foco em organização de componentes, boas práticas de hooks e comunicação com backend.

📸 Preview da aplicação

A aplicação possui duas telas principais:

Tela de Cadastro de Usuário
Tela de Listagem de Usuários
🚀 Funcionalidades
Cadastro de novos usuários
Envio de dados para API REST
Navegação entre páginas
Componentização e reutilização de UI
Interface simples, limpa e escalável
🧠 Conceitos aplicados
React Hooks (useRef, useNavigate)
Componentização
Separação de responsabilidades
Consumo de API com Axios
Estrutura de projeto escalável
🛠️ Tecnologias utilizadas
React
React Router DOM
JavaScript (ES6+)
Axios
Styled Components (ou estrutura de estilos modular)
📂 Estrutura de Pastas
src
│
├── components
│   ├── Button
│   └── TopBackground
│
├── pages
│   ├── Home
│   └── ListaUsuarios
│
├── services
│   └── api.js
│
└── styles
⚙️ Instalação e execução

Clone o repositório:

git clone https://github.com/seu-usuario/seu-repo.git

Entre na pasta do projeto:

cd seu-repo

Instale as dependências:

npm install

Execute o projeto:

npm run dev
# ou
npm start
🔌 Configuração da API

O projeto espera uma API rodando com a rota:

POST /usuarios

Payload enviado:

{
  "name": "Nome do usuário",
  "age": 25,
  "email": "email@email.com"
}

Certifique-se de configurar corretamente a baseURL no arquivo:

src/services/api.js

Exemplo:

import axios from "axios";

export default axios.create({
  baseURL: "http://localhost:3000"
});
