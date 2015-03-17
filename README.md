# Nginx PHP5 FPM UNIX Socket Configuration

Proper Nginx PHP5-FPM UNIX Socket Configuration To Avoid Bad Gateway and Timeout Errors like :

connect() to unix:/var/run/php5-fpm.sock failed 

upstream timed out ( : Connection timed out) 

connect() to unix:/tmp/php5-fpm.sock failed ( : No such file or directory)

Full Guide : https://thecustomizewindows.com/2015/03/ubuntu-nginx-php5-fpm-unix-socket-configuration/

You'll not get the whole stuff anywhere as a single piece. If `php5-fpm.sock` is not present, how much you edit `/etc/php5/fpm/pool.d/www.conf`, it will never work.
Next, `nginx` must be a member of `www-data` user group. The Gateway errors on WordPress Nginx PHP5-FPM are usually due to Nginx Microcache. 

It will work on :

PHP PHP 5.5.9 and above (CLI) + 
+ Ubuntu Nginx Community Edition 
  or Ubuntu Nginx Plus Trial 
  or Ubuntu Nginx Plus Full


Thanks : Thanks to Nginx Plus team for the smallest hint towards Microcache related problem. 

Usage Limititation : You should pay us for commercial usage. It is under GNU GL 3.0. If you drink my blood to earn money, I have no problem but think a bit about Karma. 

