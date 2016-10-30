# Daemo-Forum
The Daemo-Forum is a custom installation of [Discourse](https://github.com/discourse/discourse/) running on Heroku.
It works as:

- a mailing list
- a discussion forum
- a long-form chat room

## Requirements

Discourse is built for the *next* 10 years of the Internet, so our requirements are high:

| Browsers | Tablets |  Smartphones |
| -------- | ------- | ----------- |
| Safari 6.1+| iPad 2+ |  iOS 7+ |
| Google Chrome 23+ |  Android 4.3+ | Android 4.3+ |
| Internet Explorer 11+ | Windows 8 | Windows Phone 8 |
| Firefox 16+ | |

## Built With

- [Ruby on Rails](https://github.com/rails/rails) &mdash; Our back end API is a Rails app. It responds to requests RESTfully in JSON.
- [Ember.js](https://github.com/emberjs/ember.js) &mdash; Our front end is an Ember.js app that communicates with the Rails API.
- [PostgreSQL](http://www.postgresql.org/) &mdash; Our main data store is in Postgres.
- [Redis](http://redis.io/) &mdash; We use Redis as a cache and for transient data.

Plus *lots* of Ruby Gems, a complete list of which is at [/master/Gemfile](/).

## Setting up Daemo-Forum

1. If you're **brand new to Ruby and Rails**, please see [**our Vagrant Developer Section**](docs/VAGRANT.md), which includes a development environment in a virtual machine.

2. If you're familiar with how Rails works and are comfortable setting up your own environment, use our [**Daemo-Forum Advanced Developer Section**](docs/DEVELOPER-ADVANCED.md).

Before you get started, ensure you have the following minimum versions: [Ruby 2.0.0+](http://www.ruby-lang.org/en/downloads/), [PostgreSQL 9.3+](http://www.postgresql.org/download/), [Redis 2.6+](http://redis.io/download). If you're having trouble, please see our [**TROUBLESHOOTING GUIDE**](docs/TROUBLESHOOTING.md) first!

## Local Setup
--to do--

## Vagrant Setup
--to do--

## Heroku Setup
--to do--

## Contributing
=======

Daemo-Forum is **100% free** and **open source**. We encourage and support an active, healthy community that
accepts contributions from the public &ndash; including you!

1. Fork Daemo-Forum and clone your forked repository on your system
1. Make sure you have an `upstream` remote: `$ git remote add upstream https://github.com/crowdresearch/Daemo-Forum.git`
1. Merge the latest master from upstream: `$ git pull upstream master`
1. Create a new branch out off master for your fix/feature. `git checkout new-feature master`
1. Make your changes
1. Push your branch to your origin: `$ git push origin new-feature`
1. Make pull request against `develop` branch. :)

Most times the merge will occur without conflicts and you can proceed with PR/deployment. In the case of conflicts you will need to resolve them before proceeding.

Most conflicts occur in a consistent set of files, namely `Gemfile` and the various `Gemfile.lock` derivatives and any file heavily modified to run on Heroku such as `production.rb`, and a few controllers and javascript files. The conflicts are often the result of an addition made in our fork, so resolving the conflict is a matter of ensuring the addition is preserved while still incorporating the new functionality from upstream.

Once all conflicts are resolved, commit the changes: `$ git add . && git commit -m "Merge w/ upstream"`.

We look forward to seeing your pull requests!

Copyright 2014 - 2016 Civilized Discourse Construction Kit, Inc.
