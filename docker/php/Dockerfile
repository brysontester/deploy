# Gunakan versi PHP yang sesuai dengan kebutuhan aplikasi Laravel Anda
FROM php:8.2-fpm

# Instalasi dependensi dan MySQL client
RUN apt-get update \
    && apt-get install -y default-mysql-client \
    && docker-php-ext-install pdo_mysql

# Lakukan perintah lain yang dibutuhkan, misalnya:
# COPY . /var/www
# RUN chown -R www-data:www-data /var/www

# Set working directory
WORKDIR /var/www

# Port yang perlu di-expose (jika diperlukan)
EXPOSE 9000

# Perintah untuk menjalankan PHP-FPM
CMD ["php-fpm"]

# Tambahkan perintah tambahan yang diperlukan untuk konfigurasi aplikasi Anda
