# data-package-examples

A place to experiment with data packages

Each data package is in its own directory with a structure

```
my-data-package-directory
  |
  |- data
  |    |
  |    |- my-data.csv
  |    |- more-data.csv
  |
  |- datapackage.json
  |- README.md

```

Each data package:

- was originally produced by [Data Curator](https://github.com/ODIQueensland/data-curator)
- may have been hand-edited if Data Curator produced incorrect result. The difference between the original and hand-edited version will help improve Data Curator
- follows the [Frictionless Data](http://frictionlessdata.io) [specification](http://frictionlessdata.io/specs/)
- will be automatically validated by [Goodtables.io](http://goodtables.io)

## Adding a datapackage

On your computer:

- create a data package using Data Curator
- use the `Export Data Package` command to create a `datapackage.zip`
- rename `datapackage.zip` to my-data-package-name.zip
- unzip the files
- add all the files to this repository

## Add Goodtables.io validation

- All data in this repo is: [![goodtables.io](https://goodtables.io/badge/github/Stephen-Gates/data-package-examples.svg)](https://goodtables.io/github/Stephen-Gates/data-package-examples)
- It would be nice to have [individual badges for each data package](https://github.com/Stephen-Gates/data-package-examples/issues/1)
