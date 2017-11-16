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

- create a data package using Data Curator (it's best if the datapackage `name` is unique across this repository)
- use the `Export Data Package` command to create a `datapackage.zip`
- rename `datapackage.zip` to *my-data-package-name*.zip
- unzip the files
- add all the files to this repository

## Add Goodtables.io validation

- All data in this repo is: [![goodtables.io](https://goodtables.io/badge/github/Stephen-Gates/data-package-examples.svg)](https://goodtables.io/github/Stephen-Gates/data-package-examples)
- It would be nice to have [individual badges for each data package](https://github.com/Stephen-Gates/data-package-examples/issues/1)

## View a data package

Go to [Data Package Viewer](http://data.okfn.org/tools/view) and enter the url of one of the `datapackage.json` files, e.g.

http://data.okfn.org/tools/view?url=https%3A%2F%2Fraw.githubusercontent.com%2FStephen-Gates%2Fdata-package-examples%2Fmaster%2Fone-csv-file%2Fdatapackage.json

## Publish a data package to datahub.io

- Use [data-desktop](https://github.com/datahq/data-desktop/releases) to install [datahub-cli](https://github.com/datahq/datahub-cli)
- use the following commands to privately publish to [datahub.io](http://datahub.io) ([docs](http://datahub.io/docs), [blog](http://datahub.io/blog))

```
$ cd my-data-package-directory
$ data push
```
