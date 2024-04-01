# API REST - CITAS

Lab project 5. api rest in java springboot


## API Reference

#### Get all items

```http
  GET http://localhost:8181/users
```
returns a json with all the items

#### Post item

```http
  POST http://localhost:8181/users
```
json structura:

```json
{
     "id": 1,
     "nombre": "ususario",
     "cuenta": "usario01@gmail.com",
     "clave": "1242",
     "rol": "actor"
}
```
returns a json with the new item added

#### Delete item

```http
  DELETE http://localhost:8181/users/{id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `Long` | **Required**. Id of item to fetch |

returns a answer "true" or "false"

## Run Locally

Clone the project

```bash
  git clone https://github.com/DereckFernandoBaldiviezoCruz/Lab5_SIS324
```

Modify file: "application.properties", at your preference

```bash
  spring.datasource.url=jdbc:mysql://localhost:3306/database
  spring.datasource.username= root
  spring.datasource.password= contraseña
```