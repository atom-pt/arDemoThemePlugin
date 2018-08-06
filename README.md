# MOA theme

# Install instructions

## 1. Goto your AtoM plugins dir, by default:

cd /usr/share/nginx/atom/plugins

## 2. Get Theme plugin files from github

sudo git clone https://github.com/atom-pt/arMoaThemePlugin.git

sudo chown -R www-data:www-data arMoaThemePlugin

## 3. Make main.less

cd /usr/share/nginx/atom/plugins/arMoaThemePlugin

sudo make

## 4. Refresh and restart services

php /usr/share/nginx/atom/symfony cc

service php7.0-fpm restart

service memcached restart

service nginx restart
