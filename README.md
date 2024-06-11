# Meu Projeto de Cadastro e Login

Este é um projeto básico de sistema de cadastro e login usando Java e MySQL.

## Configuração

1. Configure o banco de dados MySQL:
    ```sql
    CREATE DATABASE cadastro_login_db;

    USE cadastro_login_db;

    CREATE TABLE usuarios (
        id INT AUTO_INCREMENT PRIMARY KEY,
        nome VARCHAR(100) NOT NULL,
        email VARCHAR(100) NOT NULL UNIQUE,
        senha VARCHAR(100) NOT NULL
    );
    ```

2. Atualize a classe `DatabaseConnection.java` com suas credenciais do banco de dados.

3. Compile e execute o projeto:
    ```bash
    mvn clean install
    mvn exec:java -Dexec.mainClass="com.seu_pacote.App"
    ```

## Dependências

- Java 8 ou superior
- MySQL
- Maven
