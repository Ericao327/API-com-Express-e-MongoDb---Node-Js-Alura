# API REST com Express e MongoDB

> Uma aplicação de API REST desenvolvida com Node.js, Express e MongoDB durante o curso de API REST com Express e MongoDB da Alura.

## 📚 Sobre o Curso

Este projeto foi desenvolvido como parte do curso **[Node.js: API REST com Express e MongoDB](https://cursos.alura.com.br/course/node-js-api-rest-express-mongodb)** da Alura.

O curso aborda os conceitos fundamentais para criar uma API REST robusta e escalável utilizando tecnologias modernas do ecossistema Node.js.

## 🛠️ Tecnologias Utilizadas

- **Node.js** - Runtime JavaScript
- **Express** - Framework web minimalista
- **MongoDB** - Banco de dados NoSQL
- **Mongoose** - ODM (Object Document Mapper) para MongoDB
- **JavaScript** - Linguagem de programação

## ✨ Funcionalidades

- ✅ CRUD completo (Create, Read, Update, Delete)
- ✅ Validações de dados
- ✅ Tratamento de erros
- ✅ Integração com banco de dados MongoDB
- ✅ Endpoints RESTful bem estruturados
- ✅ Middleware de autenticação e validação

## 🚀 Como Instalar e Executar

### Pré-requisitos

- Node.js instalado (versão 14+)
- MongoDB instalado e rodando localmente ou acesso a um servidor MongoDB remoto
- Git para clonar o repositório

### Passos para Instalação

1. **Clone o repositório:**
```bash
git clone https://github.com/Ericao327/API-com-Express-e-MongoDb---Node-Js-Alura.git
cd API-com-Express-e-MongoDb---Node-Js-Alura
```

2. **Instale as dependências:**
```bash
npm install
```

3. **Configure as variáveis de ambiente:**
Crie um arquivo `.env` na raiz do projeto com as configurações necessárias:
```
MONGODB_URI=mongodb://localhost:27017/seu_banco_de_dados
PORT=3000
```

4. **Inicie o servidor:**
```bash
npm start
```

O servidor estará rodando em `http://localhost:3000`

## 📖 Como Usar

### Exemplos de Requisições

#### GET - Obter todos os registros
```bash
curl http://localhost:3000/api/recursos
```

#### POST - Criar um novo registro
```bash
curl -X POST http://localhost:3000/api/recursos \
  -H "Content-Type: application/json" \
  -d '{"nome": "Exemplo", "descricao": "Uma descrição"}'
```

#### GET - Obter um registro por ID
```bash
curl http://localhost:3000/api/recursos/:id
```

#### PUT - Atualizar um registro
```bash
curl -X PUT http://localhost:3000/api/recursos/:id \
  -H "Content-Type: application/json" \
  -d '{"nome": "Atualizado"}'
```

#### DELETE - Deletar um registro
```bash
curl -X DELETE http://localhost:3000/api/recursos/:id
```

## 📁 Estrutura do Projeto

```
API-com-Express-e-MongoDb---Node-Js-Alura/
├── src/
│   ├── models/           # Modelos de dados (Mongoose)
│   ├── routes/           # Rotas da API
│   ├── controllers/      # Controladores de lógica
│   ├── middleware/       # Middlewares customizados
��   └── app.js            # Configuração principal da aplicação
├── .env                  # Variáveis de ambiente (não versionar)
├── .gitignore            # Arquivos a ignorar no Git
├── package.json          # Dependências do projeto
├── package-lock.json     # Lock das dependências
└── README.md             # Este arquivo
```

## 📚 Aprendizados Principais

- Criação de rotas e endpoints RESTful
- Conexão e integração com MongoDB
- Utilização de middlewares no Express
- Tratamento de requisições HTTP (GET, POST, PUT, DELETE)
- Validação e sanitização de dados
- Tratamento de erros
- Boas práticas em desenvolvimento de APIs
- Estruturação de projetos Node.js

## 👤 Autor

- **Eric** - [@Ericao327](https://github.com/Ericao327)

## 🔗 Links Úteis

- [Documentação Express](https://expressjs.com/)
- [Documentação MongoDB](https://docs.mongodb.com/)
- [Documentação Mongoose](https://mongoosejs.com/)
- [Curso Alura](https://cursos.alura.com.br/course/node-js-api-rest-express-mongodb)

---
