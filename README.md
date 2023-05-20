# jwt-refresh-token
Step-1: SignUp
{
    "name": "nur",
    "email": "nurzamal0077@gmail.com",
    "password": "anyPWD",
    "roles": "ROLE_ADMIN"
}
Step-2; login
{
    "username": "nur",
    "password": "anyPWD"
}

Step-3: getAllProducts
Get Req: localhost:8080/products/all

Step-4: once Token will expire after 3 minutes
then Request for refresh the token
Post req: localhost:8080/products/refreshToken
{
    "token": "this refresh token will get from login or in refreshtoken table in the db"
}
