<h2 align="center">
  <img alt="Banner"
       src="https://res.cloudinary.com/vinicius998609604/image/upload/v1586305968/Semana%20OmniStack%2011.0%20-%20BE%20THE%20HERO/rsxp_rsboij.png" alt="Banner"/>
</h2>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/vinicius-pimenta/rsxp-api.svg">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/vinicius-pimenta/rsxp-api.svg">
  <img alt="Repository size" src="https://img.shields.io/github/repo-size/vinicius-pimenta/rsxp-api">
  <a href="https://github.com/vinicius-pimenta/rsxp-api/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/vinicius-pimenta/rsxp-api">
  </a>
  <img alt="License" src="https://img.shields.io/badge/license-MIT-brightgreen">
   <p align="center">
    <img alt="App RS/XP" src="https://img.shields.io/badge/App-RS/XP-informational">
    <img alt="Node.js" src="https://img.shields.io/badge/Node.js-v12.16.1-informational?logo=Node.JS">
    <img alt="React" src="https://img.shields.io/badge/Adonis-v4.1.0-blue">
  </p>
</p>

<p>
  <img alt="Banner"
       src="https://res.cloudinary.com/vinicius998609604/image/upload/v1586304111/Semana%20OmniStack%2011.0%20-%20BE%20THE%20HERO/screen-1_hlthrg.jpg" width="400" align="left" />
</p>

## :large_blue_circle: Sobre

O RS/XP é um app que foi usado na Rocketseat Experience 2019. Esse app permite o usuário visualizar todas as informações do evento, como também cadastrar no workshop.

## :bust_in_silhouette: Quem ministrou?

O curso foi ministrado pelo [Diego Fernandes](https://github.com/diego3g)

## :rocket: Tecnologias

[Node.js][nodejs] | [Adonis](https://adonisjs.com/) | [NPM](https://www.npmjs.com/) | [Yarn](https://yarnpkg.com/) | [SQLite3](https://www.npmjs.com/package/sqlite3) | [PostgreSQL](https://www.postgresql.org/) | [Eslint](https://eslint.org/)

## :information_source: Como usar?

```bash
# Instala Git:
$ sudo apt update
$ sudo apt install git

# Instala Node.js & NPM:
$ sudo apt update
$ curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
$ sudo apt-get install -y nodejs
```

[Referência](https://github.com/nodesource/distributions/blob/master/README.md) usada para instalar Node.js & NPM em distribuições baseadas em Debian e Ubuntu.

<br></br>

```bash
# Instala o Docker:
$ sudo apt install docker.io

# Instala o pgAdmin4:
$ wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
$ sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" >> /etc/apt/sources.list.d/pgdg.list'
$ sudo apt-get update
$ sudo apt install pgadmin4 pgadmin4-apache2
```

[Anotações de aula](https://www.notion.so/Autentica-o-com-Adonis-com-TDD-6eb9664a0f0b481c96bf36b5c59b1799)

### :star: Após ter feito as instalações, digita na sua linha de comando:

### :gear: API

```bash
# Entra no repositório:
$ cd rsxp/

# Entra na pasta backend:
$ cd backend/

# Instala as dependências::
$ npm install
$ yarn install

# Execute o comando do Docker: Observação: o kartoza é modificado para suportar algumas funcionalidades que não são possíveis no original, como por exemplo o UUID.
$ sudo docker run --name rsxp -p 5432:5432 -d -t kartoza/postgis

# Copie o arquivo .env.example e renomeie a cópia para .env. Após isso, preencha as informações necessárias dele.
```

<img src="https://res.cloudinary.com/vinicius998609604/image/upload/v1586341151/Semana%20OmniStack%2011.0%20-%20BE%20THE%20HERO/env_isjo2v.png" align="left">

```bash
# Execute o comando adonis key:generate para gerar APP_KEY no arquivo .env. Este será usado por exemplo para gerar os hash das senhas dos usuários.
$ adonis key:generate

# Roda as migrations. Observação: certifique-se de que o PostgreSQL esteja configurado e iniciado:
$ adonis migration:run

# Verifica as rotas disponíveis na api:
$ adonis route:list

# Execute a aplicação:
$ adonis serve
```

### :heavy_check_mark: Testes automatizados

```bash
# Caso queira rodar os testes, abra outro terminal e entra na pasta backend:
$ adonis test

# Caso queira rodar os testes com o coverage, abra outro terminal e entra na pasta backend:
$ yarn test
```

## :memo: Licença

Esse projeto está sob a licença MIT. Veja a [LICENÇA](./LICENSE) para mais informação.

---

Feito com ♥ por Vinicius Pimenta :wave: [Entrem em contato!](https://www.linkedin.com/in/vinicius-pimenta-195b04181/)

[nodejs]: https://nodejs.org/
[npm]: https://www.npmjs.com/
