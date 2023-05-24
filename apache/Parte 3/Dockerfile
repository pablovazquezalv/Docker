FROM ubuntu:22.04


# Instalar Apache y otras dependencias
RUN apt-get update && apt-get install -y apache2

# Copiar la configuración del servidor
COPY settings.conf /etc/apache2/sites-available/

# Habilitar el sitio
RUN a2ensite settings.conf && a2dissite 000-default.conf

# Exponer el puerto 80
EXPOSE 80

# Ejecutar Apache en primer plano
CMD ["apachectl", "-D", "FOREGROUND"]
