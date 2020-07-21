https://medium.com/@ger86/how-to-integrate-docker-into-a-symfony-based-project-f06164dc7944

## Install
    docker-compose up -d --build

## Start the PHP container
    docker exec -it  symfony-docker_php_1 bash

## Install Symfony in the container
    curl -sS https://get.symfony.com/cli/installer | bash
    mv /root/.symfony/bin/symfony /usr/local/bin/symfony
    rm -R ../symfony/
    symfony new symfony --dir=/var/www/symfony

## Access the site
    http://localhost: 8001