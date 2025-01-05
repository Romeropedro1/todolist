# TodoList - Gerenciador de Tarefas

## Descrição

O **TodoList** é um sistema de gerenciamento de tarefas simples, desenvolvido com **Java** e o framework **Spring Boot**. A aplicação permite que os usuários possam adicionar, editar e excluir tarefas, além de marcar as tarefas como concluídas. O sistema também se conecta a um banco de dados **MySQL** e utiliza **Flyway** para controle de migrações de banco de dados.

## Tecnologias e Linguagens Utilizadas

- **Linguagem**: Java
- **Spring Boot**: Framework principal para a construção da aplicação.
- **Spring Data JPA**: Para interação com o banco de dados relacional.
- **MySQL**: Banco de dados utilizado para persistência das tarefas.
- **Flyway**: Para migração e versionamento do banco de dados.
- **bcrypt**: Para hash de senhas.
- **Lombok**: Para simplificação do código com anotações como `@Getter`, `@Setter`, `@NoArgsConstructor`, etc.

## Funcionalidades

- **Gerenciamento de Tarefas**:
  - Adicionar novas tarefas.
  - Editar e excluir tarefas.
  - Marcar tarefas como concluídas.
  
- **Autenticação**:
  - Utiliza o **bcrypt** para hash de senhas (embora a autenticação não esteja explicitamente configurada no `POM.xml`, pode ser integrada ao sistema com segurança).
  
- **Banco de Dados**:
  - **MySQL** como banco de dados para armazenar as tarefas.
  - **Flyway** para gerenciar e versionar o banco de dados, aplicando migrações de forma automática.

## Dependências

O projeto usa as seguintes dependências:

- `spring-boot-starter-data-jpa`: Para persistência com JPA (Java Persistence API).
- `spring-boot-starter-web`: Para criação de endpoints RESTful.
- `spring-boot-devtools`: Ferramentas para desenvolvimento (recarregamento automático).
- `spring-boot-starter-test`: Ferramentas para testes automatizados.
- `mysql-connector-java`: Driver JDBC para o MySQL.
- `flyway-core` e `flyway-mysql`: Para controle e execução de migrações de banco de dados.
- `bcrypt`: Para hash de senhas.
- `hibernate-core`: Core do framework Hibernate.
- `jackson-databind`: Para serialização e desserialização de JSON.
- `lombok`: Para simplificação do código com anotações.

## Como Rodar o Projeto

### Pré-requisitos

- **Java 17** ou superior.
- **MySQL**: Um banco de dados MySQL em funcionamento. Caso não tenha o MySQL instalado, você pode instalar e configurar um banco de dados local.
  
  - Crie um banco de dados chamado `todolist` no MySQL:
    ```sql
    CREATE DATABASE todolist;
    ```

- **Maven**: Para compilar e rodar o projeto.

### Passos

1. Clone o repositório:
   ```bash
   git clone https://github.com/Romeropedro1/todolist.git
