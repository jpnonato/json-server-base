# json-server-hamburgueria

Essa é uma API que foi criada para efetivar a operacionalização do projeto da hamburgeria Kenzie 2.0 

## Endpoints

A API tem um total de 4 endpoints, onde o usuário consegue se cadastrar, fazer login/logout no app. Ao logar é mostrada o catalogo dos produtos e o usuário poderá adicionar/remover um produto do catalogo na lista do seu carrinho(só ele pode ter acesso)

O url base da API é https://json-server-hamburgeria.herokuapp.com/

### Rotas que não precisam de autentificação:

### Cadastro de usuário

POST /register

{
  "email": "xxx@gmail.com",
  "password": "yyyyyy"
}

os campos obrigatórios são os de E-mail e password.Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Fazer login

POST /login 

{
	"email": "xxx@gmail.com",
	"password": "yyyyyy"
}


### Rotas que precisam de autentificação:

### Visualizar os produtos do catalogo

GET /home

### pegar um produto específico do catálogo

GET /home?name="o que fou digitado no input de pesquisa" 

### Listar as propriedades de um usuário específico

GET  /users/ id 

### alterar os dados de um usuário específico na API

Patch /users/ id



