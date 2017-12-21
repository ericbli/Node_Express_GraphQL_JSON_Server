# Node_Express_GraphQL_JSON_Server

$ npm install

$ npm run json:server
open http://localhost:3000/customers

open one more cmd window to start GraphQL server
$ npm run dev:server 
open http://localhost:4000/graphql

using GraphQL and JSON-Server
---------------------------------------------------------
{ customers {
   id, name,age
 }  }
---------------------------------------------------------
{ customer(id:"4"
  ) {
   id, name,age
 }  }
---------------------------------------------------------
mutation{
 addCustomer(
name: "Tom Jones",
   email: "tom@gmail.com",
    age: 23
  ) {
    id,
    name
  }}
---------------------------------------------------------
mutation{
 editCustomer(
  id:"2"
name: "Tom Jones",
   email: "tom@gmail.com",
    age: 1000
  ) {
   id
 } }
---------------------------------------------------------
mutation{
 deleteCustomer(
  id:"2"
  ) {
   id
 } }
 ----------------------------------------------------------
