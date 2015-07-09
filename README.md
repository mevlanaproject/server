# Mevlana Server


| URL    | Method  | Parameters | Description |
|-----------|--------|--------|---------|
| http://localhost/mevlana/v1/register   | POST   | name, email, password    | User registration     |
| http://localhost/mevlana/v1/login   | POST   | email, password   | User login     |
| http://localhost/mevlana/v1/posts | POST | post, type  | Create New Post    |
| http://localhost/mevlana/v1/posts | GET |    | Fetching All Posts    |
| http://localhost/mevlana/v1/posts | GET |    | Fetching User Posts    |
| http://localhost/mevlana/v1/posts/:postid | GET |    | Fetching Single Post    |
| http://localhost/mevlana/v1/posts/:postid | PUT | post, status, type  | Updating Post    |
| http://localhost/mevlana/v1/posts/:postid | DELETE |   | Deleting Post    |
| http://localhost/mevlana/v1/comments/:postid | POST | comment  | Create New Comment    |
| http://localhost/mevlana/v1/comments/:postid | GET |   | Fetching Post Comments    |
| http://localhost/mevlana/v1/comments/:postid/:commentid | PUT | comment,status  | Updating Comment    |
| http://localhost/mevlana/v1/comments/:postid/:commentid |  DELETE |   | Deleting Comment    |

## User Registration

### Registration response

```json
{
   "error":false,
   "message":"You are successfully registered"
}
```

## User Login

### Login response

```json
{
   "error":false,
   "apiKey":"4c7064a939fe1691e872ceb4ccb15dd5",
   "user":{
      "name":"asil",
      "email":"asilarslan93@gmail.com",
      "createdAt":"2015-07-08 19:27:40"
   }
}
```

##License
MIT
