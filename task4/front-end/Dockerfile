FROM nginx:latest

# Copy front-end files to the desired location in the container
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy custom Nginx config
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

EXPOSE 9000
