# Big Game Survey 
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/GustavoSC1/dspesquisa/blob/master/LICENSE) 

# Sobre o projeto

https://dspesquisa-gustavo.netlify.app/

Big Game Survey é uma aplicação full stack web e mobile construída durante a 1ª edição da **Semana DevSuperior** (#sds1), evento organizado pela [DevSuperior](https://devsuperior.com "Site da DevSuperior").

A aplicação consiste em uma pesquisa de preferência de games, onde os dados são coletados no app mobile, e depois são listados no app web, que também apresenta um dashboard com gráficos baseados nestes dados.

## Layout mobile
![Mobile 1](https://ik.imagekit.io/gustavosc/dspesquisa/iPhone_8_Plus_-_INTRO_da3lWM6oX.jpg) ![Mobile 2](https://ik.imagekit.io/gustavosc/dspesquisa/iPhone_8_Plus_-_FORM_N44DhDPp1.jpg)

## Layout web
![Web 1](https://ik.imagekit.io/gustavosc/dspesquisa/INTRO_9DpDg-94D.jpg)

![Web 2](https://ik.imagekit.io/gustavosc/dspesquisa/LISTA_UdjcBIqf4.jpg)

![Web 3](https://ik.imagekit.io/gustavosc/dspesquisa/GR_FICOS_0_1MrtAMU.jpg)

## Modelo conceitual
![Modelo Conceitual](https://ik.imagekit.io/gustavosc/dspesquisa/modelo-conceitual_6nzpJQ2f1.png)

# Tecnologias utilizadas
## Back end
- [Java](https://www.oracle.com/java/)
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
- [Maven](https://maven.apache.org/)
## Front end
- HTML / CSS
- [JavaScript](https://www.javascript.com/)
- [TypeScript](TypeScript)
- [ReactJS](https://pt-br.reactjs.org/)
- [React Native](https://reactnative.dev/)
- [Apex Charts](https://apexcharts.com/)
- [Expo](https://expo.io/)
## Implantação em produção
- [Back end: Heroku](https://dashboard.heroku.com/)
- [Front end web: Netlify](https://www.netlify.com/)
- [Banco de dados: Postgresql](https://www.postgresql.org/)

# Como executar o projeto

## Pré-requisitos

Para executar este projeto no modo de desenvolvimento, você precisará ter um ambiente básico para executar um Aplicativo React-Native e uma Aplicação ReactJS, que pode ser encontrado [aqui](https://www.youtube.com/playlist?list=PLNuUvBZGBA8kMTSPMmmNiRm2z0gRxXxox).

Além disso, para executar o back-end em seu computador, você também precisará ter um ambiente básico. Você pode encontrar tudo que precisa para iniciar o back-end [aqui](https://www.youtube.com/playlist?list=PLNuUvBZGBA8kMTSPMmmNiRm2z0gRxXxox).

## Back end
Pré-requisitos: Java 11

Para executar este projeto, você precisará mudar o ambiente do projeto para modo de teste. Para fazer isso vá para o arquivo /src/main/resources e edite o valor de spring.profiles.active.

Deve ser assim:

spring.profiles.active=test

```bash
# clonar repositório
git clone https://github.com/GustavoSC1/dspesquisa

# entrar na pasta do projeto back end
cd backend

# executar o projeto
./mvnw spring-boot:run
```

## Front end web
Pré-requisitos: npm / yarn

Você pode utilizar o back-end funcionando em sua máquina ou o deploy dele no Heroku, para isso acesse os arquivos src/pages/Records/index.tsx e src/pages/Charts e edite o valor de BASE_URL.

Deve ser assim:

const BASE_URL = 'https://dspesquisa-gustavo.herokuapp.com';

Ou

const BASE_URL = 'http://localhost:8080';

```bash
# clonar repositório
git clone https://github.com/GustavoSC1/dspesquisa

# entrar na pasta do projeto front end web
cd front-web

# instalar dependências
npm install

# executar o projeto
npm start
```

## Front end mobile
Pré-requisitos: npm / yarn

Você pode utilizar o back-end funcionando em sua máquina ou o deploy dele no Heroku, para isso acesse o arquivo src/pages/CreateRecord/index.tsx e edite o valor de BASE_URL.

Deve ser assim:

const BASE_URL = 'https://dspesquisa-gustavo.herokuapp.com';

Ou

const BASE_URL = 'http://localhost:8080';

Para executar o front ent mobile você também precisará baixar o aplicativo Expo em seu smartphone e utilizá-lo para ler o QR Code que vai aparecer no terminal quando terminar o start da aplicação.

```bash
# clonar repositório
git clone https://github.com/GustavoSC1/dspesquisa

# entrar na pasta do projeto front end web
cd front-mobile

# instalar dependências
npm install

# executar o projeto
npm start
```

# Autor

Gustavo da Silva Cruz

https://www.linkedin.com/in/gustavo-silva-cruz-20b128bb/
