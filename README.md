<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios-new.png" />

<h3 align="center">
  Desafio 02: Conceitos do Node.js
</h3>

## O desafio 

O desafio pede para criar uma aplicação e treinar oque foi aprendido em conceitos de Node.JS
Nele devemos armazenar repositórios, permitiremos listagem, atualização e remoção, e estes repositórios podem receber 'Likes'.

Foi propos 5 rotas com suas respectivas funções: 

- [x] POST/repositories
    A rota deve receber alguns atributos como ``` title, url, techs ``` dentro do body da aplicação, e assim cadastrar o repositório. Também salvamos um ``` id ``` no formato ``` "uuid" ``` e um atributo de ```likes``` como valor padrão 0.

- [x] GET/repositories
    A rota deve listar todos os repositórios.

- [x] PUT/repositories/:id
    Nessa rota devemos alterar os atributos  ``` title, url, techs ``` do repositório com o ``` id ``` que recebemos como Parâmetro.

- [x] DELETE/repositories/:id
    Nessa rota devemos deletar o repositório com o ``` id ``` que recebemos como Parâmetro.

- [x] POST/repositories/:id/like
    A ultima rota da aplicação foi interessante, logo abaixo deixarei o método que usei para fazer este desafio, era preciso adicionar um like no repositório em específico.

## Minha solução

A ultima rota que precisava adicionar likes em um repositório eu peguei o ```id``` e com ele fiz um ```findIndex```. Tendo o index na mão utilizei o seguinte método: ```repositories[repositoryIndex].likes++;```, tendo o array de repositórios em mãos e o index específico posso acessa-lo facilmente e manipular seus atributos. Sendo assim finalizei o desafio.

### Para instalar e usar esta aplicação sigas os passos abaixo.

1. Faça um ```git clone``` do projeto.

2. Instale as dependências do projeto utilizando ```npm install``` ou ```yarn add```.

3. Inicie o projeto com ```yarn dev```.