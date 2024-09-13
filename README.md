# CursoReactivoTransactions

Este es un microservicio desarrollado en spring webflux con una base de datos mongodb, proyecto reactivo.

- ## Para probar la solución tenemos los siguientes médotods

- ### CalculateFees

url = "http://localhost:8090/calculateFees"

payload = json.dumps({
  "Id": "10001",
  "amount": 5000
})
headers = {
  'Content-Type': 'application/json'
}

- ### Execute Batch

url = "http://localhost:8090/executeBatch"

payload = json.dumps([
  {
    "id": "1",
    "amount": 500,
    "fee": 10
  },
  {
    "id": "2",
    "amount": 1000,
    "fee": 20
  },
  {
    "id": "3",
    "amount": 1500,
    "fee": 30
  }
])
headers = {
  'Content-Type': 'application/json'
}

- ### Process Transactions

url = "http://localhost:8090/processTransactions"

payload = json.dumps([
  {
    "id": "1",
    "amount": 800,
    "fee": 10
  },
  {
    "id": "2",
    "amount": 1000,
    "fee": 20
  },
  {
    "id": "3",
    "amount": 1500,
    "fee": 30
  }
])
headers = {
  'Content-Type': 'application/json'
}