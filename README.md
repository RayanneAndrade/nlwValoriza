![banner](https://user-images.githubusercontent.com/61299540/123202984-020f5000-d48c-11eb-8c12-38af40aae04e.png)

# NLW Valoriza (Next Level week - 6ª edição) 🚀
[![nodejs-badge][nodejs-img]][nodejs]

[nodejs-img]: https://img.shields.io/badge/Node.js-v14.17-green
[nodejs]: https://nodejs.org/en/

---

## Índice 📖
* __[Descrição](#description)__
* __[Tecnologias](#technologies)__
* __[Rotas atuais](#routes)__
* __[Regras do projeto](#rules)__
* __Aulas__
  * __[Aula 1 - Criando projeto](#class1)__
  * __[Aula 2 - Criando estrutura de usuários](#class2)__
  * __[Aula 3 - Criando estrutura de tags](#class3)__
  * __[Aula 4 -  Criando estrutura de elogios](#class4)__
  * __[Aula 5 - Finalizando projeto](#class5)__

---

## Descrição 📌 <a name="description"></a>
Sistema para fazer elogio a outros usuários por meio de tags. 

--- 

## Tecnologias 💻 <a name="technologies"></a>
* __[Node.js](https://nodejs.org/en/)__ - Baixe a versão recomendada LTS.
* __[Yarn](https://classic.yarnpkg.com/en/docs/install/#windows-stable)__ - Gerenciador de pacotes, similar ao npm do Node.js.
* __[Express](https://expressjs.com/pt-br/)__ - Framework para desenvolver back-end com Node.js.
* __[TypeScript](https://www.typescriptlang.org/)__ - É JavaScript com tipagem de dados e recursos adicionais, voltado ao lado servidor.
* __[Beekeeper](https://www.beekeeperstudio.io/)__ - Gerenciador de Banco de Dados e editor de código SQL.
* __[Insomnia](https://insomnia.rest/)__ - É um programa que testa as requisições de uma API(GET, POST, PUT, DELETE, PATCH, etc).

---

## Regras do projeto <a name="rules"></a>

- **Cadastro de usuário**

- [x] Não é permitido cadastrar mais de um usuário com o mesmo em-mail

- [x] Não é permitido cadastrar usuário sem e-mail

- **Cadastro de TAG**

- [x] Não é permitido cadastrar tag sem nome

- [x] Não é permitido cadastrar mais de uma tag com o mesmo nome

- [x] Não é permitido o cadastro por usuários que não sejam administradores

- **Cadastro de elogios**
 
- [x] Não é permitido um usuário cadastrar um elogio para si

- [x] Não é permitido cadastrar elogios para usuários inválidos

- [x] O usuário precisar estar autenticado na aplicação

--- 

### Comandos básicos:

#### Inicialização e download de dependências
* __yarn init -y__ -> inicializa *package.json* no seu projeto. *-y*, no final do comando, faz o cadastro dos dados de nome, versão, main e licença automaticamente.
* __yarn tsc --init__ -> inicializa o TS.
* __yarn tsc__ -> converte TS para JS para o Node.js executar. O Node.js não compreende o TypeScript.
* __yarn add typescript -D__ -> adiciona o TypeScript em mode de desenvolvimento, quando for pra produção, o código será convertido para JavaScript.
* __yarn add express__ -> adiciona o framework express no projeto.
* __yarn add @types/express -D__ -> baixa as tipagens do express em modo de desenvolvimento.
* __yarn add ts-node-dev -D__ -> essa biblioteca converte arquivos TS em JS automaticamente, para não ficar criando arquivos com a extensão *.js* toda vez que queremos executar o projeto.

#### Execução
* __yarn dev__ -> Uma forma curta para executar o servidor na porta 3000. Definimos o comando *dev* dentro de "scripts", no package.json. Essa propriedade recebe o comando: *ts-node-dev src/server.ts*. Com essa configuração, não precisamos digitar *yarn ts-node-dev src/server.ts* toda vez que executarmos o projeto, somente yarn dev, agilizando o desenvolvimento.

--- 

### Instalação 
* _yarn add typeorm reflect-metadata sqlite3_ -> baixa as 3 dependências de uma vez(). *reflect-metadata* nos permite adicionar os *decorators*(@) as classes e funções, lhes atribuindo um apelido.


### Migrations 
  É um controle de versionamento de código SQL. Mantem a versão mais recente dos códigos do Banco de dados, assim todo time usa a mesma versão. Nesse projeto, é usado o TypeORM Migrations.

