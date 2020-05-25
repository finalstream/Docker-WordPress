# イメージを"php"でタグ"7.4-apache"で使う
FROM php:7.4-apache
# php.iniを置き換える(オプション)
# COPY ./php.ini /usr/local/etc/php/

# ライブラリをインストール(必要に応じて変更)
RUN apt-get update && apt-get install -y \
 libfreetype6-dev \
 libjpeg62-turbo-dev \
 libpng-dev \ 
 libonig-dev \
 && apt-get clean

# PHP拡張モジュールをインストール(必要に応じて変更)
RUN docker-php-ext-install pdo_mysql mysqli gd iconv