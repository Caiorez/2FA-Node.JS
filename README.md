# 2FA-Node.JS
## Requisitos de Compilação

É Necessário que seja instalado o NPM + NodeJS + Express + Nunjucks + Nexmo + Body-Parser para que os comandos abaixo funcionem.
Para realizar a instalação, visite https://www.npmjs.com/get-npm

## Configurações

É necessário fazer um cadastro no site [Vonage](http://developer.nexmo.com/ed?c=blog_text&ct=2020-07-17-how-to-add-two-factor-authentication-with-node-js-and-express)
Ao se cadastrar, pegar sua API KEY e a SECRET KEY e inserir no código a baixo

``` bash
# /index.js
const nexmo = new Nexmo({
  apiKey: 'YOUR API KEY',
  apiSecret: 'YOUR SECRET KEY',
});
```

## Compilação do Site

``` bash
# Instalação de Dependencias
npm install
npm install express
npm install nunjucks
npm install nexmo
npm install body-parser

# Se você quiser testar antes de subir para produção.
node index.js
