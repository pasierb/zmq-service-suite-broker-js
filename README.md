[![Build Status](https://travis-ci.org/micro-toolkit/zmq-service-suite-broker-js.svg?branch=master)](https://travis-ci.org/micro-toolkit/zmq-service-suite-broker-js)
[![Code Climate](https://codeclimate.com/github/micro-toolkit/zmq-service-suite-broker-js/badges/gpa.svg)](https://codeclimate.com/github/micro-toolkit/zmq-service-suite-broker-js)
[![Coverage](https://codeclimate.com/github/micro-toolkit/zmq-service-suite-broker-js/coverage.png)](https://codeclimate.com/github/micro-toolkit/zmq-service-suite-broker-js)
[![Issue Count](https://codeclimate.com/github/micro-toolkit/zmq-service-suite-broker-js/badges/issue_count.svg)](https://codeclimate.com/github/micro-toolkit/zmq-service-suite-broker-js)
[![Dependency Status](https://gemnasium.com/micro-toolkit/zmq-service-suite-broker-js.svg)](https://gemnasium.com/micro-toolkit/zmq-service-suite-broker-js)
![Grunt](https://cdn.gruntjs.com/builtwith.png)

## ZMQ Service Oriented Suite - Node-js Broker

[![NPM version](https://badge.fury.io/js/zmq-service-suite-broker.svg)](http://badge.fury.io/js/zmq-service-suite-broker)

This project is a node-js broker implementation for [Micro toolkit](http://micro-toolkit.github.io/info/) and it respects with the [zss specification](http://micro-toolkit.github.io/zmq-service-suite-specs/).

The broker is slipt in three main components:
* backend: Receives requests and replies from services;
* frontend: Receives requests and replies from clients;
* smi: Service management interface, it handles service lifecycle with smi requests: up, down, heartbeat.

## Running Broker

**ZeroMQ Install**

You need to have [0MQ installed](http://zeromq.org/area:download).

If you use MacOS just do

    $ brew install zeromq

**ZSS Broker Execution**

    $ npm install
    $ npm start


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Bump versioning

We use [grunt bump package](https://www.npmjs.org/package/grunt-bump) to control package versioning.

Bump Patch version

    $ grunt bump

Bump Minor version

    $ grunt bump:minor

Bump Major version

    $ grunt bump:major

## Running Specs

    $ npm test

## Coverage Report

We aim for 100% coverage and we hope it keeps that way! :)
We use pre-commit and pre-push hooks and CI to accomplish this, so don't mess with our build! :P

Check the report after running npm test.

    $ open ./coverage/lcov-report/index.html
