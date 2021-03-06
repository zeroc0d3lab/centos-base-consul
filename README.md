# CentOS Base Consul Docker (Base-Consul Container)
[![Build Status](https://travis-ci.org/zeroc0d3lab/centos-base-consul.svg?branch=master)](https://travis-ci.org/zeroc0d3lab/centos-base-consul) [![](https://images.microbadger.com/badges/image/zeroc0d3lab/centos-base-consul.svg)](https://microbadger.com/images/zeroc0d3lab/centos-base-consul "Layers") [![](https://images.microbadger.com/badges/version/zeroc0d3lab/centos-base-consul.svg)](https://microbadger.com/images/zeroc0d3lab/centos-base-consul "Version") [![GitHub issues](https://img.shields.io/github/issues/zeroc0d3lab/centos-base-consul.svg)](https://github.com/zeroc0d3lab/centos-base-consul/issues) [![GitHub forks](https://img.shields.io/github/forks/zeroc0d3lab/centos-base-consul.svg)](https://github.com/zeroc0d3lab/centos-base-consul/network) [![GitHub stars](https://img.shields.io/github/stars/zeroc0d3lab/centos-base-consul.svg)](https://github.com/zeroc0d3lab/centos-base-consul/stargazers) [![GitHub license](https://img.shields.io/badge/license-GPLv2-blue.svg)](https://raw.githubusercontent.com/zeroc0d3lab/centos-base-consul/master/LICENSE)

## Docker Compose
* Copy `env-example` to `.env`
* Build & running
  ```
  docker-compose build && docker-compose up
  ```
* Force recreate container
  ```
  docker-compose build && docker-compose up --force-recreate base-consul
  ```
* Running container only
  ```
  docker-compose up
  ```

## Environments
You can run docker-compose for different environment with selected containers
* Copy `env.sh.example` to `env.sh`
* Change to execute script
  ```
  chmod a+x env.sh
  ```
* Change environment in `env.sh` file
  ```
  ENV="development"            # (use: "development" or "production" as selected environment)
  CONTAINER_PRODUCTION="..."   # (selected containers will be run in production environment)
  CONTAINER_DEVELOPMENT="..."  # (selected containers will be run in development environment)
  ```
* Running script
  ```
  ./env.sh
  ```

## License
[**GNU General Public License v2**](https://github.com/zeroc0d3lab/centos-base-consul/blob/master/LICENSE)