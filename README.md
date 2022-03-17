# API Desafio React Native

Utilize essa API para contrução da sua aplicação para o Desafio de React Native da Eduzz.

Este projeto utiliza json-server, para mais informações de como utiliza-lo acesse a [documentação do json-server](https://github.com/typicode/json-server).

<p>&nbsp;</p>

## Getting started

Primeiro instale o json-server globalmente

```
npm install -g json-server
```

Agora é só rodar o servidor

```bash
json-server --watch db.json --port 8000
```

E se acessar [http://localhost:8000/withdrawals/1](http://localhost:3000/withdrawals/1), você receberá:

```json
{
  "id": 1,
  "value": 220,
  "createdAt": "2022-03-15T14:48:00.000Z"
}
```

## Rotas


```
GET    /withdrawals
GET    /withdrawals/1
POST   /withdrawals
PUT    /withdrawals/1
PATCH  /withdrawals/1
DELETE /withdrawals/1
```



### Paginação

Utilize `_page` e opicionalmente `_limit` para paginar os dados a serem retornados (por padrão são retornados 10 itens)


```
GET /withdrawals?_page=7
GET /withdrawals?_page=7&_limit=20
```


