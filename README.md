[![tests](https://github.com/drud/ddev-redis/actions/workflows/tests.yml/badge.svg)](https://github.com/drud/ddev-redis/actions/workflows/tests.yml) ![project is maintained](https://img.shields.io/maintenance/yes/2022.svg)

## What is this?

This repository allows you to quickly add [selenium standalone chrome](https://github.com/SeleniumHQ/docker-selenium) to a [Ddev](https://ddev.readthedocs.io) project.

## Installation

1. `ddev get thunder/ddev-selenium-chrome`
2. `ddev restart`

## Explanation

This selenium standalone chrome recipe for [ddev](https://ddev.readthedocs.io) installs a [`.ddev/docker-compose.selenium.yaml`](docker-compose.selenium.yaml) using the `selenium/standalone-chrome:latest` docker image.

## Interacting with Selenium standalone chrome

* The selenium chrome instance will listen on TCP port 4444.
* For debugging use `selenium/standalone-chrome-debug:latest` image and add port mapping for vnc, reachable at `vnc://localhost:6000`, if you get a prompt asking for a password, it is: `secret`.

