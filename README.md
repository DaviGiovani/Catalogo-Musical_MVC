# Catálogo Musical MVC 🎵

Um sistema de gerenciamento de discos, artistas e gêneros musicais, desenvolvido utilizando o padrão de arquitetura MVC (Model-View-Controller) com Node.js, Sequelize, Express e EJS.

---

## Funcionalidades do Projeto

- **Gerenciamento de Discos**:
  - Adicionar, editar e excluir discos.
  - Associar discos a gêneros musicais.
  - Listar todos os discos cadastrados, com informações detalhadas (ano de lançamento, capa, faixas e gênero).

- **Gerenciamento de Artistas**:
  - Adicionar, editar e excluir artistas.
  - Associar artistas a discos existentes.
  - Listar artistas cadastrados, com informações detalhadas (nome, gênero musical, discos associados e foto).

- **Gerenciamento de Gêneros**:
  - Adicionar gêneros musicais.
  - Listar gêneros, exibindo discos e artistas associados.

- **Busca Dinâmica**:
  - Busca por discos, artistas e gêneros utilizando parâmetros como nome, título ou gênero.

---

## Tecnologias Utilizadas

- **Back-end**:
  - Node.js
  - Express
  - Sequelize ORM (PostgreSQL)
- **Front-end**:
  - EJS
  - CSS personalizado
- **Banco de Dados**:
  - PostgreSQL

---

## Como Rodar o Projeto em Sua Máquina

### Pré-requisitos

Certifique-se de ter os seguintes programas instalados em sua máquina:
1. **Node.js** (versão >= 14)
2. **PostgreSQL**
3. **Git**

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/DaviGiovani/Catalogo-Musical_MVC.git
   cd Catalogo-Musical_MVC

2. **Instale as dependências:**
   ```bash
   npm install
   
3. **Configure o Banco de Dados:**
- **Crie um banco de dados no PostgreSQL**:
   ```sql
   CREATE DATABASE catalogo_musical;
- **Configure as crendenciais do banco no arquivo .env**:
  ```env
  DB_HOST=localhost
  DB_PORT=5432
  DB_USER=seu_usuario
  DB_PASSWORD=sua_senha
  DB_NAME=catalogo_musical

4. **Execute as migrações e seeds para popular o banco de dados:**
   ```bash
   npx sequelize db:migrate
   npx sequelize db:seed:all

5. **Inicie o servidor:**
   ```bash
   npm start

6. **Acesse a aplicação no navegador:**
- Acesse o endereço http://localhost:3000.

## Estrutura do projeto
- src/
  - controllers/: Lógica de controle para cada funcionalidade.
  - models/: Modelos do banco de dados utilizando Sequelize.
  - routes/: Rotas para cada funcionalidade (discos, artistas, gêneros).
  - views/: Templates EJS para renderização das páginas.
- public/:
  - css/: Estilos personalizados.
  - js/: Lógica de front-end para busca dinâmica.
- migrations/: Arquivos para criação das tabelas no banco de dados.
- seeders/: Dados iniciais para popular o banco de dados.

## Como contribuir

1. Faça um fork do repositório.
2. Crie uma branch para sua feature:
   ```bash
   git checkout -b minha-feature
3. Faça as alterações e commit:
    ```bash
   git commit -m "Adiciona minha feature"
4. Envie para sua branch:
   ```bash
   git push origin minha-feature
5. Abra um pull request

## Licença

Este projeto está sob a licença MIT. Sinta-se à vontade para utilizá-lo e modificá-lo conforme necessário.


