# Spring graphql
- GraphQL é uma linguagem de consulta para recuperar dados de um servidor. É uma alternativa ao REST, SOAP ou gRPC de alguma forma.
- Vamos supor que desejamos buscar os dados de um livro específico, submetemos a consulta abaixo:
```
{
  bookById(id: "book-1"){
    id
    name
    pageCount
    author {
      firstName
      lastName
    }
  }
}
```
- Teremos por exemplo o retorno abaixo:
```
{
  "bookById":
  {
    "id":"book-1",
    "name":"Harry Potter and the Philosopher's Stone",
    "pageCount":223,
    "author": {
      "firstName":"Joanne",
      "lastName":"Rowling"
    }
  }
}
```
