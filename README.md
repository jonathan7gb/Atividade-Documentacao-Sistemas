# 📑 API REST - GERENCIADOR DE TAREFAS

Este projeto é uma API REST desenvolvida com Java e Spring Boot, que permite o gerenciamento de tarefas vinculadas a categorias, além de possuir CRUD de usuários e relacionar tarefas a um usuário, onde cada usuário pode possuir diversas tarefas, mas uma tarefa pode pertencer a apenas um usuário. Utiliza banco de dados em memória (H2).

---

## Funcionalidades

- CRUD de Categoria
- CRUD de Usuário
- CRUD de Tarefa vinculadas a Categoria e Usuário
- Listagem de Tarefas por categoria
- Tratamento global de exceções

---

## Tecnologias

- Java 17
- Spring Boot 3
- Spring Data JPA
- H2 Database

---

## Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/carlosfabioa/sesi-gerenciador-tarefas.git
   cd sesi-gerenciador-tarefas
   
   
## Execute o projeto com Maven:
   ./mvnw spring-boot:run
   
## Acesse os recursos:
- H2 Console: http://localhost:8080/h2-console
- JDBC URL: jdbc:h2:mem:tarefas
 
 
## Endpoints da API
| Método | URL                        | Descrição                         |
|--------|----------------------------|---------------------------------- |
| POST   | /salvarTarefa              | Criar nova tarefa(com categoriaId)|
| GET    | /listarTarefas             | Listar todas as tarefas           |
| GET    | /novo/{id}                 | Cria objeto em branco             |
| PUT    | /editarTarefa/{id}         | Atualizar tarefa                  |
| DELETE | /removerTarefa/{id}        | Excluir tarefa                    |
| GET    | /listarCategoria/{id}      | Listar categorias                 |
| POST   | /salvarCategoria           | Criar categoria                   |
| GET    | /formularioTarefaCategoria | Cria objeto em branco             |
| PUT    | /editarCategoria/{id}      | Atualizar categorias              |
| DELETE | /excluirCategoria/{id}     | Excluir categoria                 |
| POST   | /salvarUsuario             | Criar usuário                     |
| GET    | /listarUsuarios            | Listar Usuários                   |
| GET    | /formularioUsuario         | Cria objeto em branco             |
| PUT    | /editarUsuario/{id}        | Atualizar usuário                 |
| DELETE | /excluirUsuario/{id}       | Excluir usuário                   |
