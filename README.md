# 🚀 Gestão de Pessoas

> Sistema para gerenciamento e cadastro de pessoas desenvolvido em Java com integração ao banco de dados MySQL.

---

## 📌 Sobre o Projeto

Este projeto é uma aplicação de **CRUD** (*Create, Read, Update, Delete*) desenvolvida com o objetivo de praticar conceitos da linguagem **Java**, manipulação de banco de dados relacional com **MySQL** e padrão de persistência de dados.

O sistema permite gerenciar cadastros de pessoas de forma estruturada, oferecendo interface/mecanismo para inclusão, consulta, alteração e exclusão de registros.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Java
- **Banco de Dados:** MySQL
- **Conectividade:** JDBC (*Java Database Connectivity*)
- **Gerenciador de Build/IDE:** Apache NetBeans / Ant

---

## ✨ Funcionalidades

- [x] **Cadastrar:** Adicionar novas pessoas ao banco de dados.
- [x] **Listar/Consultar:** Visualizar registros de pessoas cadastradas.
- [x] **Atualizar:** Editar informações de registros existentes.
- [x] **Excluir:** Remover cadastros do banco de dados.

---

## 📂 Estrutura do Repositório

```text
Gestao-de-Pessoas/
├── src/Gestao_de_Pessoas/   # Código-fonte da aplicação Java
├── build/                   # Arquivos gerados durante a compilação
├── dist/                    # Executável/JAR gerado pelo build
├── nbproject/               # Configurações do projeto NetBeans
├── build.xml                # Script de build do Apache Ant
└── README.md                # Documentação do projeto
```

---

## ⚙️ Como Executar o Projeto

### 📋 Pré-requisitos

Antes de começar, você precisará ter instalado em sua máquina:
- [Java JDK](https://www.oracle.com/java/technologies/downloads/) (versão 8 ou superior)
- [MySQL Server](https://dev.mysql.com/downloads/mysql/) ou [XAMPP](https://www.apachefriends.org/)
- Uma IDE de sua preferência (NetBeans, Eclipse, IntelliJ IDEA ou VS Code)

### 🔧 Passo a Passo

1. **Clonar o repositório:**
   ```bash
   git clone https://github.com/VineSantos/Gestao-de-Pessoas.git
   ```

2. **Configurar o Banco de Dados:**
   - Acesse o MySQL e crie a base de dados:
     ```sql
     CREATE DATABASE gestao_pessoas;
     USE gestao_pessoas;
     
     CREATE TABLE pessoas (
         id INT AUTO_INCREMENT PRIMARY KEY,
         nome VARCHAR(100) NOT NULL,
         email VARCHAR(100),
         telefone VARCHAR(20)
     );
     ```

3. **Configurar Conexão JDBC:**
   - Abra a classe responsável pela conexão com o banco de dados (ex: `Conexao.java` ou similar no pacote `src/Gestao_de_Pessoas`).
   - Verifique se as credenciais (usuário e senha do MySQL) coincidem com o seu ambiente local.

4. **Executar a aplicação:**
   - Abra o projeto na sua IDE e execute a classe principal.

---

## 🤝 Contribuição & Licença

Sinta-se à vontade para enviar sugestões, reportar *issues* ou abrir *pull requests*.

Desenvolvido por [VineSantos](https://github.com/VineSantos) 🚀
