1.  [] install composer
>>> curl -sS https://getcomposer.org/installer -o composer-setup.php
>>> sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
>>> alias composer='/usr/local/bin/composer'
2.  [] create new lapravel app
>>> composer create-project laravel/laravel domco>>>
3.  [] Go to the project directory and start Laravel server
>>> php artisan serve
4.  [] Create a view in views directory
>>> about.blade.php
5.  [] Create a route (in web.php) that return the view about.blade.php
6.  [] Create a controller AboutController (you will find the controller in App\Http\Controllers)
>>> php artisan make:controller AboutController
7.  [] Make index funtion that return the about view
8.  Make a little menu with list of link to all the pages
9.  [] Make a little footer
10. [] Create a directory in views. Name it layouts
11. [] Create a file named master.blade.php in layouts. Add all the code that are in the about view
12. [] Add the yields in the master
>>> @yield('about')
13. [] Now, in about.blade.php just add
>>> 
@extends('layouts/master')

@section('about')
    ALL YOUR CODES
@endsection

14. [] Create a directory in layouts. Name it partials.
15. [] Create a file _headerPartial.blabe.php and add the header code.
16. [] Include the partial in the master
>>>  @include('layouts/partials/_headerPartial')