## Query

`{
  user(id: "23") {
    id,
    firstName,
    age
  }
}`

## Result

`{
  "data": {
    "user": {
      "id": "23",
      "firstName": "Bill",
      "age": 20
    }
  }
}`

## Named Query

`query findCompany{
  apple: company(id: "1"){
    id
    name
    description
  }
  google: company(id: "2"){
    id
    name
    description
  }
}`

## Query Fragment (or DRY for graphQL)

`query findCompany{
  apple: company(id: "1"){
    ...companyDetails
  }
  google: company(id: "2"){
    ...companyDetails
  }
}`

`fragment companyDetails on Company {
  id
  name
  description
}`
