## Installation wp-cli

    cd ${HOME}/yps.tools
    curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
    php wp-cli.phar --info
    chmod +x wp-cli.phar
    mv wp-cli.phar wp
    ./wp --info

## Media Regenerate

    wp plugin deactivate ewww-image-optimizer
    wp media regenerate --yes
    wp plugin activate ewww-image-optimizer