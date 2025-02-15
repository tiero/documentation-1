# PHP

Base docker image: [webdevops/php-nginx](https://hub.docker.com/r/webdevops/php-nginx/) or [webdevops/php-apache](https://hub.docker.com/r/webdevops/php-nginx/)

PHP build pack contains almost every module necessary for your applications.

By default, Nginx is used to serve your application, but if you have a `.htaccess` file in the root directory of your repository, `apache` is used to take advantage of the customs rules defined.

Composer will install all dependencies if `composer.json` is detected.

You can customize this image with environment variables, see the [docs](https://dockerfile.readthedocs.io/en/latest/content/DockerImages/dockerfiles/php-nginx.html).