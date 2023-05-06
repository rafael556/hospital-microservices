<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

 ### Functional Requirements

 O microsserviço deve permitir o cadastro de novas cirurgias com informações sobre o paciente, data, hora e tipo de cirurgia.

O microsserviço deve permitir a busca de cirurgias agendadas por data, paciente ou tipo de cirurgia.

O microsserviço deve permitir a atualização de informações de cirurgias agendadas, como data, hora e tipo de cirurgia.

O microsserviço deve permitir o cancelamento de cirurgias agendadas.

O microsserviço deve enviar notificações aos pacientes sobre a confirmação do agendamento de cirurgia.

O microsserviço deve permitir a visualização da agenda de cirurgias por parte dos profissionais de saúde autorizados.

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
