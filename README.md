<b><h2 align="center">Curso de Regressão Visual - Cypress com Percy</h2></b>
=============

Estudo sobre integração do Cypress com o Percy para execução de testes de Regressão Visual. Os testes de regressão visuais são testes de alto nível que olham qualquer alteração visual do sistema, seja em uma página específica ou em um fluxo que o usuário venha a percorrer. 

Nesse repositório foram feitos exemplos simples aprendidos no curso.

:computer: Pré-requisitos
=============

Para instalar as dependências do projeto e executar os testes automatizados, é necessário que o [Node.js](http://nodejs.org) e o [NPM](http://npmjs.com) estejam instalados em seu computador.

> As seguintes versões de ambos os sistemas foram utilizadas durante a execução dos exemplos (`node 14.17.0` e `npm 6.14.13 `).

> Ao instalar o Node.js, o NPM é automaticamente instalado.

:robot: Instalação
=============

Após clonar o repositório, acesse o diretório do mesmo e execute `npm ci` para instalar as dependências de desenvolvimento.

:key: Exportando o token do projeto criado no Percy.io
=============

Exporte como uma variável de ambiente o token do seu projeto (disponível no _dashboard_ do Percy). Veja os exemplos abaixo para sitemas Windows e Unix (Mac e Linux).

```
# Windows
$ set PERCY_TOKEN=<your token here>

# Unix(Mac e Linux)
$ export PERCY_TOKEN=<your token here>
```

> Fonte: https://docs.percy.io/docs/cypress


:heavy_check_mark: Executando os testes
=============
Execute `npm test` para executar os testes em modo _headless_.
Caso queira executar no modo interativo execute o seguinte comando:
```
percy exec -- cypress open

```
OBS: Em todos os casos é necessário que a variável de ambiente **PERCY_TOKEN** esteja acessível ao terminal que você executa o comando.

Ou , caso queira exportar a variável de ambiente em tempo de execução pode utilizar o seguinte comando:

```
export PERCY_TOKEN=[seu-token-aqui] && npx percy exec -- cypress open
```

Após isso vá para a dashboard do Percy e suas snapshots estarão lá.


Um curso da [Escola Talking About Testing](https://talkingabouttesting.coursify.me).

---
Feito com 💜 by Gisele Rosa 
