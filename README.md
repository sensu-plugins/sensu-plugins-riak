## Sensu-Plugins-riak

[ ![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-riak.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-riak)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-riak.svg)](http://badge.fury.io/rb/sensu-plugins-riak)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-riak/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-riak)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-riak/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-riak)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-riak.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-riak)

## Functionality

## Files
 * bin/metrics-riak.rb
 * bin/check-riak-ringready.rb

## Usage

**metrics-riak**

 Include only output the specified values, where exclude remove those not wanted.
 
 Only one of the four available flags will be used, where the precedence order is, -i,-I,-e,-E.
 
 If include or excluded is not manually specified, standard filtering is used.
 
 If using a file, metrics are either space separated or newline separated.

```
{
    "checks": {
        "include_usage": {
            "type": "metric",
            "command": "metrics-riak.rb -i vnode_gets vnode_puts",
            ...
        },
        "include_file_usage": {
            "type": "metric",
            "command": "metrics-riak.rb -I /some/path/include.txt",
            ...
        },
        "exclude_usage": {
            "type": "metric",
            "command": "metrics-riak.rb -e vnode_gets vnode_puts",
            ...
        },
        "exclude_file_usage": {
            "type": "metric",
            "command": "metrics-riak.rb -E /some/path/exclude.txt",
            ...
        }
    }
}
```

## Installation

[Installation and Setup](http://sensu-plugins.io/docs/installation_instructions.html)

## Notes
