FROM wordpress:latest

# Copy WordPress configuration files
COPY wp-config.php /usr/src/wordpress/
COPY wp-content /usr/src/wordpress/wp-content

# Expose the WordPress port
EXPOSE 80

# Set the working directory
WORKDIR /usr/src/wordpress/

# Command to run the WordPress container
CMD ["wp", "--allow-root", "core", "update"]
