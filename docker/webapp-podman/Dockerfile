FROM docker.io/library/nginx:stable

# Crear estructura para los certificados y autenticación
RUN mkdir -p /etc/nginx/ssl /etc/nginx/auth /usr/share/nginx/html

# Copiar archivos de contenido, certificados y configuración
COPY index.html /usr/share/nginx/html/index.html
COPY nginx.conf /etc/nginx/nginx.conf
COPY certs/nginx.crt /etc/nginx/ssl/nginx.crt
COPY certs/nginx.key /etc/nginx/ssl/nginx.key
COPY auth/.htpasswd /etc/nginx/auth/.htpasswd
