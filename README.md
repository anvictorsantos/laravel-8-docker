## Steps to initialize this project

## Tutorial's and Stack's that helped me to understand and implemente docker with laravel

1. I used this video to implement this project: https://youtu.be/dNw0M2ciZAE

   1.1 If u have the project already alive in container, use this command to get him down: docker-compose down
   1.2 After that, use this command to initialized the container again: docker-compose up -d --build
   1.3 If u want remove laravel 8 that is installaded on src/._ and install another version, use those command's:
   1.3.1 docker-compose run composer create-project laravel/laravel . "8._" --prefer-dist (composer create-project laravel/laravel {directory} "5.0.\*" --prefer-dist)
   1.3.2 Now, after that, if u want to check version u need to enter in ubuntu bash: docker exec -it lara_php /bin/sh
   1.3.3 To see laravel version: php artisan --version

2. I used this tutorial to give permission for folder storage/.\*: https://stackoverflow.com/questions/23411520/how-to-fix-error-laravel-log-could-not-be-opened

   2.1 More precisely this command in terminal: docker-compose exec php chmod -R 77 storage
