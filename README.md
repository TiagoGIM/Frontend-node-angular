# Backend-Flask-Docker

Construção de uma aplicação com três partes. O [backend](https://github.com/TiagoGIM/Backend-Flask-Docker) usando o microframework FLASK (Python), o front-end será [feito com o Angular cli]() (node.js) e os [dados persistentes](##-Banco-de-dados) ficarão em um servidor que rodará em um container (docker).
O objetivo é transformar todas as partes em containers.

## Jornada de aprendizado
Como eu sempre reclamo que os tutoriais pulam as partes que tem bug, decidi relatar neste arquivo [detalhes e bugs]() cada erro e como eu contornei(ou tentei).
Coloquei em [Temas abordados](#-Temas-abordados.) alguns links que consultei durante a realização do tutorial, a final o objetivo é entender como as coisas funcionam.
### Parte 1

## Ambiente de desenvolvimento
O desenvolvimento foi feito no windows com subsistema linux (WSL).

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.
This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 10.1.6.


## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

# Temas abordados
- Instalação de (nodeJs no WSL 2)[https://docs.microsoft.com/pt-br/windows/nodejs/setup-on-wsl2]
- Um pouco sobre Cross-Origin Resource Sharing [(CORS)](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)

