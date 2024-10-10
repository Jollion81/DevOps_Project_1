# frontend/Dockerfile
FROM nginx:alpine

# Copy the Nginx configuration file
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Copy the static HTML files
COPY templates /usr/share/nginx/html

EXPOSE 80
