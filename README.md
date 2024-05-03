## 💻 Projeto

Node API-SOLID

Neste projeto, uma API foi desenvolvida utilizando o framework Fastify, incorporando padrões de design como Repository Pattern, in-memory-database, Factory Pattern, testes unitários e E2E, além dos princípios da programação SOLID.

Para o gerenciamento do banco de dados, optou-se por utilizar Docker com PostgreSQL, empregando o ORM Prisma para facilitar as operações.

A autenticação foi implementada com JWT e Refresh Token para garantir a segurança da aplicação.

Para utilizar a API é recomendável usar POSTMAN ou Insomnia

## Iniciar docker

docker start (idDocker)

## Rodando aplicação

npm run start:dev

## Acessando Prisma Studio

npx prisma studio

## RFs (Requisitos funcionais)

- [x] Deve ser possível se cadastrar;
- [x] Deve ser possível se autenticar;
- [x] Deve ser possível obter o perfil de um usuário logado;
- [x] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
- [x] Deve ser possível o usuário obter o seu histórico de check-ins;
- [x] Deve ser possível o usuário buscar academias próximas (até 10km);
- [x] Deve ser possível o usuário buscar academias pelo nome;
- [x] Deve ser possível o usuário realizar check-in em uma academia;
- [x] Deve ser possível validar o check-in de um usuário;
- [x] Deve ser possível cadastrar uma academia;

## RNs (Regras de negócio)

- [x] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [x] O usuário não pode fazer 2 check-ins no mesmo dia;
- [x] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [x] O check-in só pode ser validado até 20 minutos após ser criado;
- [x] O check-in só pode ser validado por administradores;
- [x] A academia só pode ser cadastrada por administradores;

## RNFs (Requisitos não-funcionais)

- [x] A senha do usuário precisa estar criptografada;
- [x] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
- [x] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [x] O usuário deve ser identificado por um JWT (JSON Web Token);

