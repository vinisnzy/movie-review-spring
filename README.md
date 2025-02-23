# 🎬 **Sistema de Recomendação de Filmes Personalizado**

## 📜 **Descrição**
Este projeto é uma **API REST** desenvolvida em **Spring Boot** que permite aos usuários cadastrar filmes, avaliá-los e receber recomendações personalizadas com base em seus gostos. O sistema também oferece funcionalidades para explorar filmes populares, filtrar por gênero e ver resenhas de outros usuários.

---

## 🚀 **Funcionalidades**

### 🎞️ **Filmes**
- Cadastrar um novo filme (título, diretor, gênero, sinopse, ano de lançamento, etc.).
- Listar todos os filmes.
- Buscar um filme por ID ou título.
- Atualizar informações de um filme.
- Excluir um filme.

### 👤 **Usuários**
- Cadastrar um novo usuário (nome, email, senha, etc.).
- Listar todos os usuários.
- Buscar um usuário por ID.
- Atualizar informações de um usuário.
- Excluir um usuário.

### ⭐ **Avaliação de Filmes**
- Um usuário pode avaliar um filme com uma nota (de 1 a 5) e deixar um comentário.
- Listar todas as avaliações de um filme.
- Calcular a média de avaliações de um filme.

### 🎯 **Recomendações Personalizadas**
- Com base nos gêneros dos filmes que o usuário mais avaliou positivamente, o sistema pode recomendar outros filmes do mesmo gênero ou de gêneros similares.
- Exibir uma lista de filmes populares (com base nas avaliações médias).

### 🔍 **Exploração de Filmes**
- Filtrar filmes por gênero (ação, comédia, drama, etc.).
- Ordenar filmes por popularidade (média de avaliações) ou ano de lançamento.
- Buscar filmes por diretor ou título.

---

## 🛠️ **Tecnologias e Conceitos**
- **Spring Boot**: Para criar a aplicação.
- **Spring Data JPA**: Para operações de banco de dados.
- **DTOs**: Para transferir dados entre as camadas.
- **Validação de Dados**: Anotações como *@NotNull*, *@Size*, etc.
- **Tratamento de Exceções**: Criar respostas amigáveis para erros como "Filme não encontrado".

---

## 🔌 **Exemplo de Endpoints**

### 🎞️ **Filmes:**
- **POST** `/filmes` - Cadastra um novo filme.
- **GET** `/filmes` - Lista todos os filmes.
- **GET** `/filmes/{id}` - Busca um filme por ID.
- **PUT** `/filmes/{id}` - Atualiza um filme.
- **DELETE** `/filmes/{id}` - Exclui um filme.

### 👤 **Usuários:**
- **POST** `/users` - Cadastra um novo usuário.
- **GET** `/users` - Lista todos os usuários.
- **GET** `/users/{id}` - Busca um usuário por ID.
- **PUT** `/users/{id}` - Atualiza um usuário.
- **DELETE** `/users/{id}` - Exclui um usuário.

### ⭐ **Avaliações:**
- **POST** `/reviews` - Cria uma nova avaliação.
- **GET** `/filmes/{id}/reviews` - Lista todas as avaliações de um filme.
- **GET** `/usuarios/{id}/reviews` - Lista todas as avaliações de um usuário.

---

## 🎯 **Futuras Features**

- **Autenticação e Autorização**: Adicionar login e proteção de endpoints com **Spring Security**.
- **Testes Unitários**: Escrever testes para os serviços e controladores.
- **Paginação**: Implementar paginação nas listagens de filmes e avaliações.
- **Documentação da API**: Usar **Swagger** para documentar os endpoints.
- **Filtro por Recomendações**: O Endpoint: **GET** `/usuarios/{id}/recomendacoes` para retornar filmes recomendados para o usuário.

---

Feito com ❤️ por *vinisnzy*.

Se curtiu a ideia, bora começar! 🚀

