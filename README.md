# LESG (NLT Edition)

[![Build Status](https://travis-ci.org/renegare/lesg-nlt.png?branch=master)](https://travis-ci.org/renegare/lesg-nlt)
[![Coverage Status](https://coveralls.io/repos/renegare/lesg-nlt/badge.png)](https://coveralls.io/r/renegare/lesg-nlt)

Think simplified [Kibana][1] but "No Long Ting" interface.

## Requirements

* PHP 5.4
* composer (preferably latest)
* Elastic Search (v1.2.1+)
* Logstash (to generate logs and push to ES)
* *Something* that creates loads of logs!

## Installation

```
$ git clone https://github.com/renegare/lesg-nlt
```

## Helpful commands

```
# install dependencies
[project-root]$ composer install --prefer-dist

# install frontend deps
[project-root]$ bower install

# run sass watch locally (development)
sass-sourcemap --compass --watch public/asset/sass:public/asset/css --poll

# run website locally (development)
[project-root]$ php -S 0.0.0.0:8000 -t public/

# server side tests (tdd)
[project-root]$ vendor/bin/phpunit

# selenium browser tests (bdd)
[project-root]$ echo "NOT YET IMPLEMENTED"

# build
[project-root]$ echo "NOT YET IMPLEMENTED"
```

## Test

Check out the repo and from the top level directory run the
following command (xdebug required for code coverage):

```
$ composer update && vendor/bin/phpunit --coverage-text
```

## Road Map

- [ ] Free style

[1]: http://www.elasticsearch.org/overview/kibana/
