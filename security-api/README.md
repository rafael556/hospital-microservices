<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

### Security API

Requisitos Funcionais para o Microsserviço de Segurança:

Autenticação: O microsserviço deve fornecer um mecanismo de autenticação seguro para permitir que os usuários se autentiquem no sistema.

Autorização: O microsserviço deve implementar um mecanismo de autorização robusto que permita o controle de acesso baseado em funções, perfis ou permissões.

Gerenciamento de usuários: O microsserviço deve permitir o gerenciamento de usuários, incluindo a criação, exclusão e atualização de informações de usuário.

Registro de auditoria: O microsserviço deve ser capaz de registrar todas as atividades de usuário relacionadas à segurança e acesso, incluindo login, logout, tentativas de acesso não autorizadas e alterações de permissões.

Criptografia: O microsserviço deve ser capaz de criptografar dados confidenciais armazenados no banco de dados, como senhas de usuários e informações de pacientes.

Gerenciamento de sessão: O microsserviço deve implementar um mecanismo para gerenciar sessões de usuários, incluindo o tempo limite de sessão e o encerramento de sessões inativas.

Proteção contra ataques: O microsserviço deve incluir medidas de segurança para proteger contra ataques, incluindo prevenção de injeção de SQL, XSS e outros tipos de ataques.

Backup e recuperação: O microsserviço deve ser capaz de realizar backups regulares do banco de dados e permitir a recuperação rápida em caso de falhas ou corrupção de dados.

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation

```bash
$ yarn install
```

## Running the app

```bash
# development
$ yarn run start

# watch mode
$ yarn run start:dev

# production mode
$ yarn run start:prod
```

## Test

```bash
# unit tests
$ yarn run test

# e2e tests
$ yarn run test:e2e

# test coverage
$ yarn run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).
