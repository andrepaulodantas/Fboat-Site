# F-Boat

O projeto fboat é subdividido nos pacotes, **core**, **server** e **client**.

## Os projetos

### Core

O projeto core é um módulo compartilhado entre o backend e o frontend, nele, existe o modelo do domínio, além das interfaces de serviços obrigatórias a serem implementadas.

### Server

O projeto server é o backend da aplicação. Foi desenvolvido utilizando o microframework Fastify.

### Client

O projeto client é o frontend da aplicação. Foi desenvolvido utilizando o framework reativo ReactJs.

## Dependências do projeto
- [Docker](https://docs.docker.com/desktop/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Make](https://gnuwin32.sourceforge.net/packages/make.htm)
- [Node >= 16](https://nodejs.org/en/download/)
- Npm >= 7 (Instalado junto ao node)

## Como utlizar?

1 - Use npm outdated para descobrir dependências que estão desatualizadas.
2 - Use npm update para realizar atualizações de dependências seguras.
3 - Use npm install <packagename>@latest para atualizar para a versão principal mais recente de um pacote.
4 - Use npx npm-check-updates -u e npm install para atualizar todas as dependências para suas versões principais mais recentes.

Instale as dependências na raíz do projeto
`npm install`

#### Rodando o server

Construa o projeto
`npm run build:server`

Rode o projeto
`npm run start:server`

#### Rodando o client

Rode o projeto
`npm run start:client`

### Rodando os testes das aplicações

Testes de unidade do server
`npm run test:server`

Testes de integração do server
`npm run test:server:integration`

Testes de unidade do client
`npm run test:client`

## Troubleshooting

#### Comando make não é reconhecido

Se certifique que o Make está instalado e que a pasta de instalação está no PATH do sistema.

#### Não é possível alocar a porta 3306

Muito possívelmente você possui um servidor MySQL já rodando em sua máquina, por isso se certifique de parar o servidor e rode novamente o comando `npm run start:server`

#### O pacote `@fboat/core` não foi encontrado

Efetue um build das dependências do pacote core executando o comando `npm run build:core`# Fboat-Site
# Fboat-Site
