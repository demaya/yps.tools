## Initialitzing new wp page

### Installation yps.tools
    cd ~
    git clone https://github.com/demaya/yps.tools.git

### Installation wp-cli

    cd ${HOME}/yps.tools
    curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
    php wp-cli.phar --info
    chmod +x wp-cli.phar
    mv wp-cli.phar wp
    ./wp --info

### Test it
    cd ~/yps.tools
    ./wp-updates

## Media Regenerate

    wp plugin deactivate ewww-image-optimizer
    wp media regenerate --yes
    wp plugin activate ewww-image-optimizer
