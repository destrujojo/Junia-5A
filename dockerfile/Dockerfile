# Utiliser l'image officielle de Nginx comme image de base
FROM nginx:latest

# Mettre à jour les paquets et installer PHP, PHP-FPM et PHP-MySQL
RUN apt-get update && \
    apt-get install -y php php-fpm php-mysql && \
    rm -rf /var/lib/apt/lists/*

# Copier la configuration Nginx personnalisée si besoin (optionnel)
# COPY ./nginx.conf /etc/nginx/nginx.conf

# Commande par défaut pour démarrer Nginx
CMD php8.2-fpm && nginx -g 'daemon off;'

