[![Build Status](https://travis-ci.org/Icinga/puppet-icingaweb2.png?branch=master)](https://travis-ci.org/Icinga/puppet-icingaweb2)

# Icinga Web 2 Puppet Module

#### Table of Contents

1. [Overview](#overview)
2. [Module Description - What the module does and why it is useful](#module-description)
3. [Setup - The basics of getting started with Icinga Web 2](#setup)
    * [What Icinga Web 2 affects](#what-icinga-web-2-affects)
4. [Usage - Configuration options and additional functionality](#usage)
5. [Reference](#reference)
6. [Development - Guide for contributing to the module](#development)

## Overview
[Icinga Web 2] is the associated web interface for the open source
monitoring tool [Icinga 2]. This module helps with installing and managing
configuration of Icinga Web 2 and its modules on multiple operating systems.

### Description

This module installs and configures Icinga Web 2 on your Linux host by using the official packages from
[packages.icinga.com]. Dependend packages are installed as they are defined in the Icinga Web 2 package.

This module can manage all configurations files of Icinga Web 2 and import an initial database schema. It can install and
manage all official [modules](https://www.icinga.com/products/icinga-web-2-modules/) as well as modules developed by the
community.

## Setup

### What the Icinga 2 Puppet module supports

* Installation of Icinga Web 2 via packages
* Configuration
* MySQL / PostgreSQL database schema import
* Install and manage official Icinga Web 2 modules
* Install community modules

### Dependencies

This module depends on

* [puppetlabs/stdlib] >= 4.16.0
* [puppetlabs/vcsrepo] >= 1.3.0
* [puppetlabs/concat] >= 2.0.1

Depending on your setup the following modules may also be required:

* [puppetlabs/apt] >= 2.0.0
* [puppetlabs/yumrepo_core] >= 1.0.0
* [puppet/zypprepo] >= 2.0.0

### Limitations

This module has been tested on:

* Debian 9, 10
* CentOS/RHEL 6, 7
  * Requires [Software Collections Repository](https://wiki.centos.org/AdditionalResources/Repositories/SCL)
* Ubuntu 16.04, 18.04
* SLES 12

* PHP >= 7.0

Other operating systems or versions may work but have not been tested.

## Usage


## Reference

See [REFERENCE.md](https://github.com/Icinga/puppet-icingaweb2/blob/master/REFERENCE.md)

## Development

A roadmap of this project is located at https://github.com/Icinga/puppet-icingaweb2/milestones. Please consider
this roadmap when you start contributing to the project.

### Contributing

When contributing several steps such as pull requests and proper testing implementations are required.
Find a detailed step by step guide in [CONTRIBUTING.md].

### Testing

Testing is essential in our workflow to ensure a good quality. We use RSpec as well as Serverspec to test all components
of this module. For a detailed description see [TESTING.md].

### Release Notes

When releasing new versions we refer to [SemVer 1.0.0] for version numbers. All steps required when creating a new
release are described in [RELEASE.md]

See also [CHANGELOG.md]

### Authors

[AUTHORS] is generated on each release.


[Icinga 2]: https://www.icinga.com/products/icinga-2/
[Icinga Web 2]: https://www.icinga.com/products/icinga-web-2/

[puppetlabs/apt]: https://github.com/puppetlabs/puppetlabs-apt
[puppetlabs/yumrepo_core]: https://github.com/puppetlabs/puppetlabs-yumrepo_core
[puppet/zypprepo]: https://forge.puppet.com/puppet/zypprepo
[puppetlabs/stdlib]: https://github.com/puppetlabs/puppetlabs-stdlib
[puppetlabs/concat]: https://github.com/puppetlabs/puppetlabs-concat
[puppetlabs/vcsrepo]: https://forge.puppet.com/puppetlabs/vcsrepo
[puppetlabs/mysql]: https://github.com/puppetlabs/puppetlabs-mysql
[puppetlabs/puppetlabs-postgresql]: https://github.com/puppetlabs/puppetlabs-postgresql
[packages.icinga.com]: https://packages.icinga.com

[CHANGELOG.md]: CHANGELOG.md
[AUTHORS]: AUTHORS
[RELEASE.md]: RELEASE.md
[TESTING.md]: TESTING.md
[CONTRIBUTING.md]: CONTRIBUTING.md
