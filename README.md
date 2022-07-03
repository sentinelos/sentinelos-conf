# Sentinel OS configuration

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/sentinelos/conf)](https://github.com/sentinelos/conf/releases)

This repo contains a set of utilities for making backup of config files and for setting up a new Sentinel OS computer.

## LBU Basic usage

  * To add a file or folder to be backed up, `lbu include /path/to/foo`
  * To remove a file from being backed up, `lbu exclude /path/to/foo`
  * To setup LBU options, edit `/etc/lbu/lbu.conf`
  * To create a package as specified in lbu.conf, `lbu commit`
  * To override destination of the backup package, `lbu package /path/to/bar.apkovl.tar.gz`

## Setup scripts

The main script is called `setup-sentinelos`, and it will perform basic system setup. Each script can be called independently, for example:

  * `setup-acf` sets up ACF web interface
  * `setup-ntp` sets up NTP service
  * etc.

