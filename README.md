## Config-Merger

Allows for crazy config file setups. merges multiple files into one file.


[![Build Status](https://travis-ci.org/dlmoody/config-merger.svg?branch=master)](https://travis-ci.org/dlmoody/config-merger)
[![Code Climate](https://codeclimate.com/github/dlmoody/config-merger/badges/gpa.svg)](https://codeclimate.com/github/dlmoody/config-merger)
[![Test Coverage](https://codeclimate.com/github/dlmoody/config-merger/badges/coverage.svg)](https://codeclimate.com/github/dlmoody/config-merger/coverage)
[![Issue Count](https://codeclimate.com/github/dlmoody/config-merger/badges/issue_count.svg)](https://codeclimate.com/github/dlmoody/config-merger)
##Install

```npm install config-merger```

##Create a configuration in your package.json

Create a section in your package.json config like this

```
 "config-merger": [
    {
      "company1": {
        "output": "app.config.json",
        "srcFolder": "company1_configs"
      }
    },
    {
      "company2": {
        "output": "app.config.json",
        "srcFolder": "company2_configs"
      }
    }
  ],
  ...
```

##Command line API

Then you could set up a npm script with something like

```
 NODE_ENV=production  config-merger --config=company1
 ```

Profit !!!
