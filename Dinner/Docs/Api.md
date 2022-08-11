# Dinner API 

Table of Contents (up to date) 
- [Dinner API](#Dinner-api) 
  - [Auth](#auth) 
    - [Register](#register) 
      - [Register Request](#register-request) 
      - [Register Response](#register-response) 
    - [Login](#login) 
      - [Login Request](#login-request) 
      - [Login Response](#login-response) 

## Auth 

### Register 

```js
POST {{host}}/auth/register 
```

#### Register Request
```json
{
    "firstname": "Mithun",
    "lastname": "Howlader",
    "email": "mithun.primetechbd@gmail.com",
    "password": "1234"
}
```
#### Register Response

```js
200 ok
```

```json
{
    "id": "d89c2d9a-eb3e-4075-95ff-b920b55aa104",
    "firstname": "Mithun",
    "lastname": "Howlader",
    "email": "mithun.primetechbd@gmail.com",
    "token": "eyjhb..hbbq"
}
```

#### Login

```js
POST {{host}}/auth/login 
```

#### Login Request

```json
{
    "email": "mithun.primetechbd@gmail.com",
    "password": "123456"
}
```

#### Login Response
```js
200 ok
```

```json
{
    "id": "d89c2d9a-eb3e-4075-95ff-b920b55aa104",
    "firstname": "Mithun",
    "lastname": "Howlader",
    "email": "mithun.primetechbd@gmail.com",
    "token": "eyjhb..hbbq"
}