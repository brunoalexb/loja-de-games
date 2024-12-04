# Loja de Games 🕹️

Este é um projeto de uma aplicação backend para uma Loja de Games, desenvolvido em Java com Spring Boot. O sistema permite o gerenciamento de produtos e categorias, oferecendo um CRUD completo para ambos os recursos.

## Funcionalidades ✨

- CRUD completo para Produtos:
  - Criar, listar, buscar por ID, atualizar e excluir produtos.
  - Buscar produtos por nome.
  
- CRUD completo para Categorias:
  - Criar, listar, buscar por ID, atualizar e excluir categorias.

- Relacionamento **One-to-Many** entre Categorias e Produtos:
  - Cada categoria pode conter vários produtos.

## Tecnologias Utilizadas 🛠️

- **Java**  
- **Spring Boot**  
- **Hibernate/JPA**  
- **MySQL**  
- **Insomnia** (para testes da API)  

## Configuração do Projeto ⚙️

### Pré-requisitos
- Java 17+  
- MySQL Server  
- Uma IDE de sua escolha (Eclipse, IntelliJ, etc.)  

### Configuração do Banco de Dados
No arquivo `application.properties`, configure as seguintes propriedades:  

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/loja_de_games
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
