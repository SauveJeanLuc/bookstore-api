
<h1> 💻 Sobre o desafio </h1>

Nesse desafio, tive que criar uma aplicação para treinar a construção de uma api com `Spring Boot!`

Em resumo precisei criar uma `API REST, usando o Spring Boot com persistência usando JPA num banco de dados postgreSQL.`

Essa será uma aplicação para armazenar **`livros`** que pertencem a uma **`categoria`**, que irá permitir a criação, listagem, atualização e remoção dos livros, e além disso também irá permitir a criação, listagem, atualização e remoção de categorias, porém uma categoria só pode ser **`removida`** caso não exista nenhum livro associado.


## 🏁 A API deve disponibilizar os seguintes recursos: 


### 👉 Rotas da aplicação para uma Categoria 

- **`POST /categorias`**: A rota deve receber `nome` e `descricao` dentro do corpo da requisição.

- **`GET /categorias`**: Rota que lista todos as categorias, certifique-se de que apenas as categorias sem os seus livros estão na respostas, para isso você deve implementar um **`DTO`** para categoria;

- **`PUT /categorias/:id`**: A rota deve alterar apenas o `nome`, a `descricao` que serão recebidos no corpo da requisição, você deve encontrar no repositório um `id` igual ao `id` presente nos parâmetros da rota;

- **`DELETE /categorias/:id`**: A rota deve deletar o repositório com o `id` presente nos parâmetros da rota, certifique-se de que uma categoria só será removida se não tiver livros associados;

- **`POST /categorias/`**: A rota deve adicionar uma nova categoria, recebendo no corpo da requisição um `nome` e uma `descricao`;

<hr>

### 👉 Rotas da aplicação para um Livro

- **`POST /livros/cadastrar?categoria=1`**: A rota deve receber `titulo` e `nomeAutor` dentro do corpo da requisição, certifique-se de que o livro irá pertencer a alguma categoria, um livro não pode ser criado sem uma categoria.  

- **`GET/livros/1`**: Rota que lista um livro pelo seu `id`.

- **`GET/livros`**: Rota que lista todos os `livros`, certifique-se de que apenas o `titulo` e o `nomeAutor` do livro estarão na resposta, ou seja, a resposta não pode conter o id e o texto do livro, para isso você deve implementar um **` DTO`** para livro;

- **`PUT /livros/:id`**: A rota deve alterar apenas o `titulo`, a `nomeAutor` , que serão recebidos no corpo da requisição, você deve encontrar no repositório um `id` de um livro igual ao `id` de um livro presente nos parâmetros da rota;

- **`DELETE /livros/:id`**: A rota deve deletar o livro com o `id` de um livro presente nos parâmetros da rota.

<hr>

### 🚀 Funcionalidades criadas

- [x] Cadastro de categoria
- [x] Listagem de categoria
- [x] Listagem de categoria por `id`
- [x] Alteração de categoria por `id`
- [x] Remoção de categoria por `id`

<hr>

- [x] Cadastro de livro
- [x] Listagem de livro
- [x] Listagem de livro por `id`
- [x] Alteração de livro por `id`
- [x] Remoção de livro por `id` 




