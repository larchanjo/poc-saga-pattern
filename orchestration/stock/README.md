# Setup

## Postgres

docker run -d --name=postgres --net=host postgres:latest

# Test

### Create Stock

~~~
POST http://localhost:8082/v1/products
Accept: application/json
Content-Type: application/json

{
  "name" : "MC Donald's Big tasty",
  "value" : 20,
  "quantity" : 100
}
~~~

### List Stocks

~~~
GET http://localhost:8082/v1/products
Accept: application/json
Content-Type: application/json
~~~