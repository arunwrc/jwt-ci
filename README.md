# Rest In CI
This is a simple todo rest application based on CodeIgniter, [REST Server](https://github.com/chriskacerguis/codeigniter-restserver), [JWT Implementation](https://github.com/firebase/php-jwt).

# Setup

Step 1: Please run `composer install` in `application` directory first.<br />
Step 2: No Need to create database in mysql, just straight import DB/todo.sql in mysql. <br />
Step 3: 

# Run


Create JWT Token, please refer screenshots in Reference folder.

```
URL: http://localhost:8000/auth/token
Method: POST
Multipart Form:
    username: arunr
    password: 12345
```

Create Todo
You need to set jwt token into Authorization header, please refer screenshots in Reference folder.
```
URL: http://localhost:8000/todo
Method: POST
Multipart Form:
    user_id: 1
    todo: your todo
    done: 0
```

List Todo
```
URL: http://localhost:8000/todo
Method: GET
```

