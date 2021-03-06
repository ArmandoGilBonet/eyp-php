# php

![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

**AtlasIT-AM/eyp-php**: [![Build Status](https://travis-ci.org/AtlasIT-AM/eyp-php.png?branch=master)](https://travis-ci.org/AtlasIT-AM/eyp-php)

#### Table of Contents

1. [Overview](#overview)
2. [Module Description](#module-description)
3. [Setup](#setup)
    * [What php affects](#what-php-affects)
    * [Setup requirements](#setup-requirements)
    * [Beginning with php](#beginning-with-php)
4. [Usage](#usage)
5. [Reference](#reference)
5. [Limitations](#limitations)
6. [Development](#development)

## Overview

A one-maybe-two sentence summary of what the module does/what problem it solves.
This is your 30 second elevator pitch for your module. Consider including
OS/Puppet version it works with.

## Module Description

If applicable, this section should have a brief description of the technology
the module integrates with and what that integration enables. This section
should answer the questions: "What does this module *do*?" and "Why would I use
it?"

If your module has a range of functionality (installation, configuration,
management, etc.) this is the time to mention it.

## Setup

### What php affects

* A list of files, packages, services, or operations that the module will alter,
  impact, or execute on the system it's installed on.
* This is a great place to stick any warnings.
* Can be in list or paragraph form.

### Setup Requirements

This module requires pluginsync enabled and eyp/nsswitch module installed

### Beginning with php

```yaml
fpm:
  phpfpm:
    user: bbt-deploy
fpmpool:
  www:
    listen: 0.0.0.0:9000
    user: bbt-deploy
    env:
      APPLICATION_ENV: pro
    maxchildren: 30
    maxspareservers: 6
```

## Usage

Put the classes, types, and resources for customizing, configuring, and doing
the fancy stuff with your module here.

## Reference

Here, list the classes, types, providers, facts, etc contained in your module.
This section should include all of the under-the-hood workings of your module so
people know what the module is touching on their system but don't need to mess
with things. (We are working on automating this section!)

## Limitations

Tested on Ubuntu 14.04

## Development

We are pushing to have acceptance testing in place, so any new feature should
have some test to check both presence and absence of any feature
