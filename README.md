You can use `npm run start:dev` command in each service to start the server

## Assignment

- Create a new microservice called billing-service with an HTTP endpoint (POST /billing)

- Send the req.body object we are getting in (POST /shipping) of shipping-service using HTTP request to (POST /billing)

- console log the object in billing-service in same endpoint i.e (POST /billing)

- object should follow the following format

```
{
    "employeeId": "<your employee id>",
	"address": "lorem ipsum",
	"address2": "lorem ipsum",
	"postal": "74600",
	"city": "KHI",
	"country": "PAKISTAN"
}
```

- Write a Docker Compose file of 4 microservices (inventory-service, shipping-service, users-service, billing-service) to run each microservice independently on their ports.

PORT Numbers should follow the following convention

- inventory-service (500x) where x is the first digit of my employee number
- shipping-service (500x) where x is the second digit of my employee number
- users-service (500x) where x is the third digit of my employee number
- billing-service (500x) where x is the fourth digit of my employee number