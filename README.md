# About this Repo

This is a clone of the original official gcc image repo:
https://github.com/docker-library/gcc

The reason for this port is that the current official build is
building on top of Debian Jessie, which is shipping with glibc 2.18,
whereas I need to create portable binaries that will also run on
redhat 7, which uses glibc 2.17. Building on centos 7 would result in
binaries linked against glibc 2.17, which also run on glibc 2.18.

This image is currently building with centos 6 (EOL: Nov 30, 2020),
which links against glibc 2.12.

Please refer to the documentation on the [official image](https://docs.docker.com/docker-hub/official_repos/) for [gcc](https://registry.hub.docker.com/_/gcc/).

