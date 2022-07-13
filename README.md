# capistrano scm static zip

Support compression of dist. and uncompress to reduce deploy time for static sites.

# Installation

## Gemfile.rb

`gem 'capistrano-scm-staticzip', '~> 0.0.2', require: false`

## Capfile

```
require 'capistrano/scm/staticzip'
install_plugin Capistrano::SCM::Staticzip
```

## deploy.rb

`set :dist, 'path to your static template compilation folder'`

For eg,

set :dist, 'build' # in case for reactjs


set :dist, 'dist' # in case for vuejs
