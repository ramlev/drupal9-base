# A simple base Drupal 9 project.

## Required tools.

* Docker
* DDev

## Install

### Clone the project
    $ git clone git@github.com:ramlev/drupal9-base.git myproject

### Configure ddev / site

Change `name` in the .ddev/config.yaml

    $ vim .ddev/config.yaml

    $ ddev start

    $ # Install composer packages
    $ ddev composer install

    $ # Install simple site
    $ ddev exec drush site:install -y

    $ # Create a one-time-login, to change admin password
    $ ddev exec drush uli

    $ # Launch the site
    $ ddev launch

