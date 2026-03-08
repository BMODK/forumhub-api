# FórumHub API 🚀

Projeto desenvolvido como parte do Challenge da formação **Java e Spring Framework** no programa **Oracle Next Education (ONE)** em parceria com a **Alura**.

## 🛠️ Tecnologias Utilizadas
* **Java 17** 
* **Spring Boot 3** 
* **Spring Security** (Autenticação via JWT) 
* **MySQL** (Banco de dados)
* **Flyway** (Migração de banco de dados)
* **Lombok** 

## 📌 Funcionalidades (CRUD de Tópicos)
O sistema permite gerenciar tópicos de um fórum com as seguintes operações protegidas por autenticação:
* **Login**: Autenticação de usuários cadastrados com geração de Token JWT. 
* **Cadastrar**: Criação de novos tópicos (Validação de títulos duplicados). 
* **Listar**: Listagem paginada e ordenada de todos os tópicos. 
* **Detalhar**: Visualização completa de um tópico por ID.
* **Atualizar**: Edição de título e mensagem de tópicos existentes. 
* **Excluir**: Remoção física de tópicos do sistema. 

## 🚀 Como Executar
1. Clone o repositório.
2. Configure o arquivo `application.properties` com as credenciais do seu MySQL. 
3. Execute as migrações do Flyway para criar as tabelas. 
4. Inicie a aplicação via IntelliJ ou Terminal.

## 🔐 Segurança
Todas as rotas, exceto `/login`, exigem um **Bearer Token** válido no cabeçalho Authorization da requisição. 
