# Apache image

A apache image to run with php-fpm.
The fpm fcgi host and port must be defined via an environment
variable.

## Available Environment Vars

* APACHE_CONF_WEBMASTER
* APACHE_CONF_FCGI_HOST
* APACHE_CONF_FCGI_PORT

## Example:
`docker run --volume /my/local/document/root:/var/www/public/ --env APACHE_CONF_FCGI_HOST=the-host --env APACHE_CONF_FCGI_PORT=9000 -p 8888:80 apache-2`
