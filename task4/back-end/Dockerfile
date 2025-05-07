# Use the latest version of Nginx
FROM nginx:latest

# Copy the front-end files to the Nginx web server directory
COPY ./ /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000
EXPOSE 9000
