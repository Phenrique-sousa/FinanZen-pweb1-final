# Projeto FinanZen

**FinanZen** é uma aplicação desenvolvida com o objetivo de ajudar os usuários a organizarem suas finanças pessoais. O projeto oferece uma plataforma para cadastro, listagem, edição e exclusão de transações financeiras, com a funcionalidade de autenticação de usuários. O sistema é dividido em dois componentes principais:

- **Frontend**: Desenvolvido em Angular, onde os usuários interagem com a aplicação.
- **Backend**: Implementado com Spring para persistência dos dados- especificamente o registro de dicas.

## Funcionalidades

### Autenticação de Usuários

- O sistema utiliza o **Firebase Authentication** para gerenciar a autenticação de usuários, permitindo que cada pessoa tenha uma conta personalizada e segura.

**Usuário:** 
- Email
- Senha

### Cadastro de Transações

- Cada transação registrada está associada ao ID do usuário autenticado, gerado pelo Firebase Authentication.
- As informações sobre as transações, como nome, valor, tipo (entrada ou saída), data, categoria e descrição, são salvas no banco de dados **Firestore**, simulando um relacionamento entre os dados da transação e o usuário que a cadastrou.

### Edição e Remoção de Transações

- Os usuários podem editar e remover suas próprias transações. As alterações são refletidas diretamente no banco **Firestore**.

### Listagem de Transações

- O sistema permite a visualização de todas as transações cadastradas pelo usuário, exibindo as informações de cada transação de forma organizada, com a opção de editar ou excluir.

### Filtros de Transações

- O usuário pode aplicar filtros para visualizar transações por categoria, tipo ou período, facilitando a organização financeira.

## Tecnologias Utilizadas

- **Angular**: Framework para desenvolvimento do frontend e gerenciamento de estado da aplicação.
- **Angular Material**: Biblioteca de componentes UI para Angular, utilizada para criar uma interface amigável e responsiva.
- **Firebase Authentication**: Serviço de autenticação utilizado para gerenciar usuários e garantir que as transações sejam associadas a contas específicas.
- **Firestore**: Banco de dados NoSQL utilizado para armazenar as transações financeiras dos usuários.
- - **Java com Spring Boot**: Usado para o backend, oferecendo serviços REST para o frontend e integração com o banco de dados.
- - **PostgreSQL**: Banco de dados relacional utilizado para armazenar as informações das dicas financeiras.

## Estrutura do Projeto

O projeto está dividido em dois componentes principais:

1. **Frontend (Angular)**: Responsável pela interface com o usuário, permitindo o cadastro, edição, remoção e listagem de transações financeiras  no Firestore, garantindo uma sincronização em tempo real.
2. **Backend (Spring Boot)**: API responsável pela comunicação entre o frontend e o banco de dados, gerenciando a lógica de negócio.

## Links do Repositório

- [Projeto_FinanZen](https://github.com/cassiaagomes/Gestao_Financeira)

## Alunos Envolvidos

- [Cássia Gomes](https://github.com/cassiaagomes)
- [Heitor Sales](https://github.com/heitor-sales)
- [Pedro Henrique](https://github.com/Phenrique-sousa)
