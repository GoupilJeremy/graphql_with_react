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

`mutation {
  editUser(id: "40", age: 10){
    id
    firstName
    age
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

`{
  "data": {
    "editUser": {
      "id": "40",
      "firstName": "Alex",
      "age": 10
    }
  }
}`
