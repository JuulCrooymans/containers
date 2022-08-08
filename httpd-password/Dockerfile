FROM httpd

COPY index.html /usr/local/apache2/htdocs/index.html
COPY ./config/httpd.conf /usr/local/apache2/conf/httpd.conf
COPY ./config/.htpasswd /usr/local/apache2/htdocs/.htpasswd
COPY ./config/.htaccess /usr/local/apache2/htdocs/.htaccess