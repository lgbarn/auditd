
[![Build Status](https://travis-ci.org/lgbarn/auditd.png?branch=master)](https://travis-ci.org/lgbarn/auditd)

#### Table of Contents

1. [Overview](#overview)
2. [Module Description - What the module does and why it is useful](#module-description)
3. [Setup - The basics of getting started with auditd](#setup)
    * [What auditd affects](#what-auditd-affects)
    * [Beginning with auditd](#beginning-with-auditd)
4. [Usage - Configuration options and additional functionality](#usage)
5. [Reference - An under-the-hood peek at what the module is doing and how](#reference)
5. [Limitations - OS compatibility, etc.](#limitations)
6. [Development - Guide for contributing to the module](#development)

## Overview

This module will install a basic template for auditd rules. 
Thss should be a starting point for security auditing on your Linux server

## Module Description

This module edits the default /etc/audit/auditd.conf and adds a /etc/audit/audit.rules file to the server and restarts auditd.

## Setup

### What auditd affects

* /etc/audit/auditd.conf
* /etc/audit/audit.rules
* RPM Package audit will be installed
* Servce auditd will be turned on and started

### Beginning with auditd

Install module with `sudo puppet module install auditd` or use r10k.

## Usage

Use the following syntax to get this module working:

~~~
include auditd
~~~

or 

~~~
class { 'auditd': }
~~~

## Reference

### Classes

#### Public Classes
<<<<<<< HEAD
- `auditd`: Installs and configures auditd on your server.

<<<<<<< HEAD
####Private Classes
* [`auditd::config`](#auditdconfig): Configures the module. 
* [`auditd::install`](#auditdinstall): Installs auditd package on your server.
* [`auditd::params`](#auditdparams): Sets parameters for module.
* [`auditd::service`](#auditdservice): Configures auditd service.
=======
#### Private Classes
<<<<<<< HEAD
=======
- [`auditd`](#auditd): Installs and configures auditd on your server.

#### Private Classes
>>>>>>> e4b38a3... added space for proper markdown formatting
- [`auditd::config`](#auditdconfig): Configures the module. 
- [`auditd::install`](#auditdinstall): Installs auditd package on your server.
- [`auditd::params`](#auditdparams): Handle parameters to module.
- [`auditd::service`](#auditdservice): Configures auditd service.
>>>>>>> e4b38a3... added space for proper markdown formatting
=======
- `auditd::config`: Configures the module. 
- `auditd::install`: Installs auditd package on your server.
- `auditd::params`: Handle parameters to module.
- `auditd::service`: Configures auditd service.
>>>>>>> 5bc0cb1... added module install specifics

## Limitations

This module has only been tested on RedHat,CentOS and it derivatives. 
All other distributions are not supported.

## Development

This module is public and can be found on github[here](https://github.com/lgbarn/auditd)

