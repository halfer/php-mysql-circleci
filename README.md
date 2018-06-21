PHP and MySQL/MariaDB demo on CircleCI
===

![Build badge](https://circleci.com/gh/halfer/php-mysql-circleci.svg?style=badge)

This repository is a very small demonstration of installing a MySQL/MariaDB server on the CircleCI
continuous integration platform, installing PHP, and then making a database connection. It was originally
written to help a fellow software engineer on the [CircleCI forum](https://discuss.circleci.com/), and is
kept here to be useful to others.

This repo does not do anything useful in itself, other than teach readers how to set up this combination
of software on a CircleCI build server.

Instructions
---

1. Clone this repo to your own GitHub account

2. Get yourself a free CircleCI account, signing in with GitHub

3. Add your GitHub project using the "Add Projects" tab

4. Click the 'Start building' button

CircleCI will discover the [configuration file](.circleci/config.yml) and build according to the set-up
in there. You should get a "green build", which will say that the installation and database connection
was successful.

Support
---

If you get stuck with using this repo, please post on the CircleCI forum.

Further development
---

This config just uses one Docker image to do the build, and installs MariaDB into that container. However,
a separate Docker image could be spun up for MariaDB instead of installing it. It does not really
matter which of these approaches you take, other than you may find that one is faster than the other.
