# Ig.news

 🚀 Em construção... 

![GitHub repo size](https://img.shields.io/github/repo-size/DaniloCalegaro/ignews-nextjs)

---
### Tabela de conteúdos

- [Ig.news](#ignews)
    - [Tabela de conteúdos](#tabela-de-conteúdos)
  - [Visão Geral](#visão-geral)
    - [A Página](#a-página)
    - [Captura de Tela](#captura-de-tela)
  - [Pré-requisitos](#pré-requisitos)
- [Stripe](#stripe)
- [GitHub](#github)
- [FaunaDB](#faunadb)
  - [Autor](#autor)

## Visão Geral
### A Página

Aplicação em Next para consumo de notícias, nela é possível realizar o login pelo Github (Autenticação + [NextAuth](https://next-auth.js.org/) + [FaunaDB](https://fauna.com/)) e adquirir o acesso as notícias de acordo como o valor estipulado pelo [Stripe](https://stripe.com/br)

### Captura de Tela

![ignews](https://user-images.githubusercontent.com/33231886/177450296-a54e3377-67a7-4721-bc25-231dad6e0d99.jpg)


## Pré-requisitos

Para executar o projeto *local*, primeiramente baixamos o projeto em nosso equipamento e criamos um arquivo na pasta `ignews-nextjs` chamado `.env.local` com o seguinte conteúdo:

````
# Stripe
STRIPE_API_KEY= //** key do produto cadastrado no Stripe **//
NEXT_PUBLIC_STRIPE_PUBLIC_KEY= //** key publica do Stripe **//
STRIPE_SUCCESS_URL=http://localhost:3000/posts
STRIPE_CANCEL_URL=http://localhost:3000/

# GitHub
GITHUB_ID=//** Client ID github **//
GITHUB_SECRET=//** key github após cadastrado a aplicação a ser logada **//

# FaunaDB
FAUNADB_KEY=//** key do banco de dados Fauna criado para aplicação **//

````
Logo após salvar e executar os comandos:

> yarn install

E para iniciar a aplicação:

> yarn dev

Após estes passos a aplicação poderá ser visualizada no endereço [http://localhost:3000](http://localhost:3000)

## Autor
Linkedin - [Danilo Calegaro](https://www.linkedin.com/in/danilo-calegaro/)