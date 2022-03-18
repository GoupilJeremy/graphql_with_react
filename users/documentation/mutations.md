# Mutation

## Queries

`mutation {
  addUser(firstName: "Jeremy", age: 38) {
    id
    firstName
    age
  }
}`

`mutation {
  deleteUser(id: "79jdCGB"){
    id
  }
}`

## Responses

`{
  "data": {
    "addUser": {
      "id": "79jdCGB",
      "firstName": "Jeremy",
      "age": 38
    }
  }
}`

`{
  "data": {
    "deleteUser": {
      "id": null
    }
  }
}`
