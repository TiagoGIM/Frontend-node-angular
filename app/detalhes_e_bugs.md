# Iniciando a jornada
## 1. Parte I
Primeirio passo instalar o node e o npm no meu wsl2, segui esses topicos:
 - [Configurar o ambiente de desenvolvimento do Node.js com o WSL 2](https://docs.microsoft.com/pt-br/windows/nodejs/setup-on-wsl2).
(_Fique confortável pra tentar outras alternativas._)

Criei o repositório no github separado para este projeto na intenção de evitar problemas de versão e gerenciamento.
Nome do meu repositorio : Frontend-node-angular

Se for fazer igual basta ir no seu git, criar o rep e configurar no seu git local.

Instalei o angular cli

```
$ npm install -g @angular/cli
```

Iniciei o projeto no caso a pasta é o diretorio do git.

```
$ ng new Frontend-node-angular
$ cd Frontend-node-angular
```

A partir deste ponto estamos dentro do diretorio *"/Frontend-node-angular"*.
Iniciei as configurações do git 
```$ git init
$ git add . & git commit -m "first commit"
$ git branch -M main
$ git remote add origin https://github.com/TiagoGIM/Frontend-node-angular.git 
```

Tudo setado agora vamos consumir nossa API backend com o angular.
primeiro passo o Endpoint do servidor, criei um arquivo env.ts como indicado no tutorial.
```
$ touch src/app/env.ts
```
Em seguida criamos a pasta "exams" dentro de .scr/app ela conterá os arquivos relacionados à entidade do backend.
```
$ mkdir src/app/exams
```
Agora vamos criar os arquivos:
```
$ touch src/app/exams/exam.model.ts src/app/exams/exam-api.service.ts
```
Ambos estão comentados com suas funções aqui no rep. (De nada) 

Segui com as orientações do tutorial, copiando e colando os scripts sem alterar nada.
Até o momente de inciar a aplicação...
### bugs da primeira parte.
- Primeiro bug, não encontra o modulo "rxjs"
 Solução : instalei o modulo com o npm.
- Segundo bug apareceu. Uma incompatibilidade com o formato do get no arquivo src/app/exams/exams-api.service.ts
editei a linha que estava aparecendo o problem com .
```
get<Exam[]>(`${API_URL}/exams`)
```
Resolvi seguindo essa ajuda: [Stackoverflow link](https://stackoverflow.com/questions/54475893/typescript-type-x-is-missing-the-following-properties-from-type-y-length-pop)
