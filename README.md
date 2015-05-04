## Sensu-Plugins-riak

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-riak.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-riak)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-riak.svg)](http://badge.fury.io/rb/sensu-plugins-riak)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-riak/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-riak)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-riak/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-riak)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-riak.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-riak)
[ ![Codeship Status for sensu-plugins/sensu-plugins-riak](https://codeship.com/projects/a68be280-d4b3-0132-a281-4e043b6b23b5/status?branch=master)](https://codeship.com/projects/77865)

## Functionality

## Files
 * bin/metrics-riak
 * bin/check-riak-ringready

## Usage

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-riak -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-riak`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-riak' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-riak' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
