# Yona CMS

## Installation

Clone project with git clone

    git clone git@github.com:alexander-torosh/yona-cms.git

Make `cache` directory writable

    chmod -R a+w cache

Build Docker images

    docker-compose build

Start Docker containers in detached mode

    docker-compose up -d

### Docker container

Connect to the main Docker container

    docker exec -it yona-cms bash

### Configuration

Create environment configuration file `.env` from `.env.example`

    cp .env.example .env

### Composer

Install composer libraries

    composer install

### Assets

Install node_modules packages

    yarn install

Or with npm

    npm install

Build assets

    yarn encore dev

Or with npm

    npm encore dev

## Development

@TODO Complete this section

## Production Performance

@TODO Complete this section

## Environment configuration

**Optimize composer autoloader**

    composer dump-autoload --no-dev --classmap-authoritative
