FROM ubuntu:latest

# Update package lists
RUN apt-get update


# Create a directory for your project files
RUN mkdir -p /var/www/html/myproject

# Copy your project files to the Apache document root
COPY . /var/www/html/myproject/

# Expose port 80 (default for Apache)
EXPOSE 80

# Start Apache in the foreground (optional)
CMD ["apache2", "-f", "-H"]
