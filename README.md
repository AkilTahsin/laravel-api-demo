<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

## Project Setup

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects.

Start by the following commands in your terminal.
```bash
git clone <github-project-link>

cd project/directory/
composer install
npm install
```
Create a database in mysql.
Then update the .env file with your database information (database name, user and password).
```bash
php artisan migrate
php artisan db:seed
```
Start project server `php artisan serve` and visit your localhost IP. (Default: 127.0.0.1:8000)

------------

User Tinker to navigate DB:Model data
`php artisan tinker`
› `App\Models\Comment::all()`

## API Endpoints
`GET|HEAD api/comments` -> comments.index › Api\CommentController@index
`POST api/comments` -> comments.store › Api\CommentController@store
`GET|HEAD api/comments/{comment}` -> comments.show › Api\CommentController@show
`PUT|PATCH api/comments/{comment}` -> comments.update › Api\CommentController@update
`DELETE api/comments/{comment}` -> comments.destroy › Api\CommentController@destroy
