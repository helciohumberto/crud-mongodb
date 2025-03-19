# CRUD com Express e MongoDB

Este é um projeto de exemplo para um CRUD (Create, Read, Update, Delete) utilizando Express.js e MongoDB.

## Tecnologias Utilizadas

- Node.js
- Express.js
- MongoDB
- Mongoose
- EJS (Template Engine)

## Requisitos

- Node.js instalado
- MongoDB instalado ou acesso a um cluster do MongoDB Atlas

## Instalação

1. Clone o repositório:

   ```sh
   git clone https://github.com/seu-usuario/crud-mongodb.git
   cd crud-mongodb
   ```

2. Instale as dependências:

   ```sh
   npm install
   ```

3. Configure as variáveis de ambiente:

   Crie um arquivo `.env` na raiz do projeto e adicione:

   ```env
   PORT=3000
   MONGO_URI=mongodb://localhost:27017/nome-do-banco
   ```

4. Inicie o servidor:

   ```sh
   npm start
   ```

## Rotas Disponíveis

### Criar um novo registro

**POST** `/items`

**Corpo da requisição:**
```json
{
  "nome": "Item 1",
  "descricao": "Descrição do item"
}
```

### Listar todos os registros

**GET** `/items`

### Buscar um registro por ID

**GET** `/items/:id`

### Atualizar um registro

**PUT** `/items/:id`

**Corpo da requisição:**
```json
{
  "nome": "Novo Nome",
  "descricao": "Nova Descrição"
}
```

### Excluir um registro

**DELETE** `/items/:id`

## Estrutura do Projeto

```
crud-mongodb/
├── bin/
├── public/
├── routes/
├── views/
├── .gitignore
├── app.js
├── db.js
├── package.json
├── README.md
```

## Contribuição

Sinta-se à vontade para abrir um PR ou relatar problemas na página de issues.

## Licença

Este projeto está licenciado sob a MIT License - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

