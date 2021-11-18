# Guia de estudos React

## Guia de estudos React

### Uma biblioteca JavaScript para criar interfaces de usuário

## Deploy blogPessoal React no Heroku

## Configurando github

![enter image description here](https://i.imgur.com/VExFLu4.png)

Coloque o seu projeto react no github na pasta raiz do repositorio sem nenhuma pasta externa como esta demonstrado na imagem e no link abaixo:

https://github.com/LucasCapSilva/ReactBlogDeploy

**NÃO ESQUEÇA DE APAGAR O ARQUIVO yarn.lock como descrito na imagem e no link do repositório de exemplo.**

## Criando uma conta no heroku

![enter image description here](https://i.imgur.com/Sanio9B.png)

![enter image description here](https://i.imgur.com/Ph5Y0VY.png)

https://id.heroku.com/login

Faça o login no heroku

## Criando um app no heroku

Crie um nome  para o seu projeto **LEMBRANDO QUE O PROJETO DEVE SER UNICO E TOTALMENTE MINUSCULO**

![enter image description here](https://i.imgur.com/UFO4Jsb.png)

![enter image description here](https://i.imgur.com/iJMJlIL.png)

## Configurando o app heroku ao repositório do GitHub

![enter image description here](https://i.imgur.com/JbsAOFP.png)

![enter image description here](https://i.imgur.com/1wGcJ3t.png)


vincule o seu projeto ao github como descrito na imagem e escolha a branch para o deploy da aplicação, **recomendamos deploy na branch main.**

## Executando a aplicação heroku

![enter image description here](https://i.imgur.com/HzZq9qB.png)

![enter image description here](https://i.imgur.com/4WZz5KC.png)


**Caso de erro no build APAGAR O ARQUIVO package-lock.json tambem e refazer o build.**

![enter image description here](https://i.imgur.com/z80boId.png)

## Caso de erro persistir.

faça

**Colocar o substitua o codigo no package.json**

"scripts": {
     "dev": "react-scripts start",
     "start": "serve -s build",
     "build": "react-scripts build",
     "test": "react-scripts test --env=jsdom",
     "eject": "react-scripts eject",
     "heroku-postbuild": "npm run build"
}

**E execute o comando no terminal npm install serve --s**

**Suba a alteração no Github e execute o deploy novamente no heroku**

### Para utilizar a aplicação de forma local para manutenção coloque o script anterior no package.json

,
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
  
  **Execute npm install e npm start**
