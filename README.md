<h1 align="center">
    <img src="./.github/assets/bitcoin-logo.webp" width="50px">
    <br/>Bitcoin Candle Generator
</h1>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/CrisnaldoSantos/my-weather?color=f68a1f">

  <a href="https://www.crisnaldocarvalho.com.br">
    <img alt="Made by Crisnaldo" src="https://img.shields.io/badge/made%20by-Crisnaldo Carvalho-f68a1f">
  </a>

  <img alt="Languages" src="https://img.shields.io/github/languages/count/CrisnaldoSantos/bitcoin-candle-generator?color=f68a1f">

  <img alt="Version" src="https://img.shields.io/github/package-json/v/CrisnaldoSantos/bitcoin-candle-generator?color=f68a1f">

  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/CrisnaldoSantos/bitcoin-candle-generator?color=f68a1f">

  <img alt="node-current" src="https://img.shields.io/node/v/typescript?color=f68a1f">
</p>

## Tecnologias:

- NodeJS
- RabbitMQ

## Descrição:

<p>
Script que coleta uma amostra temporal de dados da api da <a href="https://www.coingecko.com/pt" target="_blank">coingecko</a> do preço de bitcoin para gerar uma candle, sendo avaliada a mostragem e atribuindo as cores vermelha para indicar queda e verde para indicar aumento da cotação.
</p>
<p>
Essa aplicação faz parte de um projeto de sistema distribuído, na qual após as coletas de geração da candle a mesma é enfileirada utilizando RabbitMQ, para que os dados sejam consumidos por uma api presente em outro repositório.
</p>

## Instalação:

Após clonar o repositório, instale as dependências do projeto com os comandos abaixo via terminal:

```js
cd bitcoin-candle-generator
npm install
```

Abra o projeto no seu editor de código na sua preferência, renomeie o arquivo ".env.example" para ".env" e insira a ural de api da <a href="https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd" target="_blank">Coingecko </a>, nome da fila e servidor do RabbitMQ nas váriáveis de ambiente presente no arquivo.
Com o terminal na pasta raiz do projeto, execute o comando:

```js
npm dev
```
