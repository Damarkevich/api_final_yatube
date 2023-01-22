# Team training project: api_yatube - 

## Technologies used:
Python3, Django Framework, Django Rest Framework, JWT, Djoser

## Project description:

Platform for publishing posts and comments on them. It is possible to create groups with descriptions, attach posts to groups. You can also subscribe to authors.

The project was accessed via API, changing content only by authors, creating content only for authenticated applications. View content The project uses JWT tokens for authentication.

## How to launch a project:

Clone the repository and switch to it on the command line:

```
https://github.com/Damarkevich/api_final_yatube.git
```

```
cd api_final_yatube
```

Create and activate virtual environment:

```
python3 -m venv env
```

```
source env/bin/activate
```

```
python3 -m pip install --upgrade pip
```

Install dependencies from a file:

```
pip install -r requirements.txt
```

Run migrations:

```
python3 manage.py migrate
```

Start project:

```
python3 manage.py runserver
```

## Endpoints API Yatube
```
api/v1/posts/ (GET, POST): get a list of all posts or create a new post.
```
```
api/v1/posts/{post_id}/ (GET, PUT, PATCH, DELETE): get, edit or delete a post by id.
```
```
api/v1/groups/ (GET): get a list of all groups.
```
```
api/v1/groups/{group_id}/ (GET): get information about a group by id.
```
```
api/v1/posts/{post_id}/comments/ (GET, POST): get a list of all post comments with id=post_id or create a new one by specifying the id of the post we want to comment on.
```
```
api/v1/posts/{post_id}/comments/{comment_id}/ (GET, PUT, PATCH, DELETE): get, edit or delete a comment by id for a post with id=post_id.
```
```
api/v1/follow/ (GET, POST): get a list of all subscriptions or create a new subscription.
```
``` 
api/v1/jwt/create/ (POST): we pass the login and password, we get the token.
```
```
api/v1/jwt/refresh/ (POST): pass a refresh token, get a new access token.
```
```
api/v1/jwt/verify/ (POST): verifying the token.```
```
In response to POST, PUT, and PATCH requests, the API returns the object that was added or changed.

## Project author
```
Dmitrii Markevich
github: https://github.com/Damarkevich/
```