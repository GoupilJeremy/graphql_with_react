# Mutation

## Query

`mutation {
  addUser(firstName: "Jeremy", age: 38) {
    id
    firstName
    age
  }
}`

## Response

`{
  "data": {
    "addUser": {
      "id": "79jdCGB",
      "firstName": "Jeremy",
      "age": 38
    }
  }
}`
