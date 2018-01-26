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

Data packages:

- were originally produced by [Data Curator](https://github.com/ODIQueensland/data-curator) unless noted in the `README.md` for that data package
- may have been hand-edited if Data Curator produced incorrect result. The difference between the original and hand-edited version will help improve Data Curator
- follow the [Frictionless Data](http://frictionlessdata.io) [specification](http://frictionlessdata.io/specs/)
- are automatically validated by [Goodtables.io](http://goodtables.io)

## Adding a data package

On your computer:

- create a data package using Data Curator (it's best if the data package `name` is unique across this repository)
- use the `Export Data Package` command to create a `datapackage.zip`
- rename `datapackage.zip` to *my-data-package-name*.zip
- unzip the files
- add all the files to this repository
- update goodtables.yml to include the data package in the automatic validation

## Add Goodtables.io validation

- Collectively the data packages in this repository are: [![goodtables.io](https://goodtables.io/badge/github/Stephen-Gates/data-package-examples.svg)](https://goodtables.io/github/Stephen-Gates/data-package-examples)
- If the data is not valid, [get details of the errors at goodtables.io](https://goodtables.io/github/Stephen-Gates/data-package-examples)
- the validation performed is controlled by [goodtables.yml](https://github.com/Stephen-Gates/data-package-examples/blob/master/goodtables.yml)
- It would be nice to have [individual badges for each data package](https://github.com/Stephen-Gates/data-package-examples/issues/1)

## View a data package

- Go to [Data Package Viewer](http://data.okfn.org/tools/view) and enter the url of one of the `datapackage.json` files
- here's [an example](http://data.okfn.org/tools/view?url=https%3A%2F%2Fraw.githubusercontent.com%2FStephen-Gates%2Fdata-package-examples%2Fmaster%2Faustralian-open-data-portals%2Fdatapackage.json)

## Publish a data package to datahub.io

- Use [data-desktop](https://github.com/datahq/data-desktop/releases) to install [datahub-cli](https://github.com/datahq/datahub-cli)
- use the following commands to publish to [datahub.io](http://datahub.io) ([docs](http://datahub.io/docs), [blog](http://datahub.io/blog))

```
$ cd my-data-package-directory
$ data push
```

## Issues and requests

[Report a bug](/issues/new?template=bugs.md&labels=bug) or [Request a new feature](/issues/new?template=feature-request.md&labels=enhancement)
