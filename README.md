# json-server-base

A API possui 4 endpoints, register, login, hobby e jobs

### Cadastro

POST /register <br/>

Para realizar o registro é necessário informar o email e a senha da seguinte maneira:<br/>
{<br/>
"email": "exemplo@email.com",<br/>
"password":"123456"<br/>
}<br/>

### Login

POST /login <br/>

A realizção do login deve ser feita de maneira análoga ao de registro, passando as mesmas informações:<br/>
{<br/>
"email": "exemplo@email.com",<br/>
"password":"123456"<br/>
}<br/>

### Hobby

-> Cadastro

POST /hobby <br/>

Para cadastrar um hobby é necessário a autorização pelo token, e o cadastro é feito da seguinte maneira:<br/>

{<br/>
"title": "Exemplo",<br/>
"frequencia": "Exemplo",<br/>
"userId": 1 (id do usuário)<br/>
}<br/>

-> Visualização

GET /hobby <br/>

Não há necessidade de o usuário estar logado para visualização<br/>

### Job

-> Cadastro

POST /job <br/>

Para cadastrar um job é necessário a autorização pelo token, e o cadastro é feito da seguinte maneira:<br/>

{<br/>
"title": "Exemplo",<br/>
"company": "Exemplo",<br/>
"userId": 1 (id do usuário)<br/>
}<br/>

-> Visualização

GET /job <br/>

É necessário a autorização pelo token para visualização<br/>
