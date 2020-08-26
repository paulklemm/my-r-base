# This project is retired

# my-r-base

This is a fork of r[ocker-org/rocker](https://github.com/rocker-org/rocker) [r-base](https://github.com/rocker-org/rocker/tree/master/r-base) but with a stable [debian](https://hub.docker.com/_/debian) release as base-image.

I will try to keep it up to date with [r-base:latest](https://github.com/rocker-org/rocker/tree/master/r-base/latest).

## Why not r-base

I rely on r-base in my mytidyverse docker image, which contains all kinds of different software I use for my data science work in R.

I struggled a lot with changing debian package dependencies every time I upgrade to a new r-base version.
Therefore I decided to fork the r-base code and only change the input image.
If there is an easier way of doing this, please let me know.

## History

- *2020-08-26*
  - Retired project. I've discovered that doing `rm -rf /etc/apt/apt.conf.d/default` is doing the trick for reverting the apt-get source to the debian default.
- *2020-08-25*
  - Initial commit, started the project
