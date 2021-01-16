1.  [] install composer
<curl -sS https://getcomposer.org/installer -o composer-setup.php>
<sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer>
<alias composer='/usr/local/bin/composer'>
2.  [] create new lapravel app
<composer create-project laravel/laravel domco>
3.  [] Go to the project directory and start Laravel server
<php artisan serve>
4.  [] Create a view in views directory
<about.blade.php>
5.  [] Create a route (in web.php) that return the view about.blade.php
6.  [] Create a controller AboutController (you will find the controller in App\Http\Controllers)
<php artisan make:controller AboutController>
7.  [] Make index funtion that return the about view