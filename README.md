# vesta-php-fpm-82
VestaCP PHP templates for PHP 8.2

Usage:

```
apt-get install php8.2-apcu php8.2-mbstring php8.2-bcmath php8.2-cli php8.2-curl php8.0-fpm php8.2-gd php8.2-intl php8.2-mysql php8.2-soap php8.2-xml php8.2-zip php8.2-memcache php8.2-memcached
update-rc.d php8.2-fpm defaults
a2enconf php8.2-fpm
systemctl restart apache2
cp -r /etc/php/8.2/ /root/vst_install_backups/php8.2/
rm -f /etc/php/8.2/fpm/pool.d/*
wget https://github.com/t0rik/vesta-php-fpm-82/raw/master/PHP-FPM-82.stpl -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-82.stpl
wget https://raw.githubusercontent.com/t0rik/vesta-php-fpm-82/main/PHP-FPM-82.tpl -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-82.tpl
wget https://raw.githubusercontent.com/t0rik/vesta-php-fpm-82/master/PHP-FPM-82.sh -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-82.sh
chmod a+x /usr/local/vesta/data/templates/web/apache2/PHP-FPM-82.sh
```
