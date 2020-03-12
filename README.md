# Cygnus-Labs Docker-Compose WordPress

WordPress powered by Docker! Now run WordPress anywhere you can install Docker.

## Installing / Getting started

This project depends on

1. [Git](https://git-scm.com/downloads)
2. [Docker](https://docs.docker.com/engine/installation/)
3. [Docker Compose](https://docs.docker.com/compose/install/)

_We're working on getting the dependencies installed by the install script. In
the meantime, please install the dependencies manually._

This project has an installer script that will install it locally.

You can fetch that script, and then execute it locally. It's well documented so that you can read through it and understand what it is doing before you run it.

```shell
curl -fsSL https://github.com/nico-swan-cygnus-labs/provisioner_wordpress_docker/master/scripts/setup -o setup.sh
bash setup.sh
```

## Usage

1. Create a WordPress site

```shell
cygnus-labs create example.com --wp
```

2. Delete a site
```shell
cygnus-labs delete example.com
```

3. Use wp-cli with a site
```shell
cygnus-labs wp example.com theme list
```

4. Create a Wordpress Site with SSL
```shell
cygnus-labs create example.com --wp --le
```

Run `cygnus-labs --help` for all commands.

## Configuration

The sites get created at `/var/www`. You can view and change the configuration
for any of the sites at `/var/www/SITE/config`

Run `cygnus-labs restart SITE` to load new configuration.

## Contributing

If you'd like to contribute, please fork the repository and use a feature
branch. Pull requests are warmly welcome.

## Licensing

The code in this project is licensed under MIT license. See [Licence](https://github.com/nico-swan-cygnus-labs/provisioner_wordpress_docker/blob/master/LICENSE)
for more information.
