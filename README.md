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
spring.jpa.hibernate.ddl-auto=update
spring.jpa.database=mysql
spring.datasource.url=jdbc:mysql://localhost/db_lojagames?createDatabaseIfNotExist=true&serverTimezone=America/Sao_Paulo&useSSl=false
spring.datasource.username=seuuser
spring.datasource.password=suasenha
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.MySQLDialect

spring.jpa.properties.jakarta.persistence.sharedCache.mode=ENABLE_SELECTIVE

spring.jackson.date-format=yyyy-MM-dd HH:mm:ss
spring.jackson.time-zone=Brazil/East
```
### Como executar o projeto

1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/loja-de-games.git
```

2. Importe na sua IDE
3. Configure o arquivo application.properties com suas credenciais do banco de dados.
4. Execute a aplicação.

Testando a API 📋

Utilize o **Insomnia** ou outra ferramenta para realizar as requisições.

### Endpoints para Produtos
- **POST** `/produtos` - Adiciona um novo produto.
- **GET** `/produtos` - Retorna todos os produtos.
- **GET** `/produtos/{id}` - Retorna um produto pelo ID.
- **PUT** `/produtos/{id}` - Atualiza um produto existente.
- **DELETE** `/produtos/{id}` - Exclui um produto pelo ID.
- **GET** `/produtos/nome/{nome}` - Retorna produtos pelo nome.

### Endpoints para Categorias
- **POST** `/categorias` - Adiciona uma nova categoria.
- **GET** `/categorias` - Retorna todas as categorias.
- **GET** `/categorias/{id}` - Retorna uma categoria pelo ID.
- **PUT** `/categorias/{id}` - Atualiza uma categoria existente.
- **DELETE** `/categorias/{id}` - Exclui uma categoria pelo ID.
- **GET** `/categorias/descricao/{descricao}` - Retorna categorias pela descrição.

Autor 🧑‍💻
Feito por Bruno Alexandre.
