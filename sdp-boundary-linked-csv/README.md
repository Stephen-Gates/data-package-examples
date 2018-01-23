Country Population referencing official boundaries using a codelist

An attempted implementation of the boundary-linked data proposal made in [Spatial Data Package Investigation](https://research.okfn.org/spatial-data-package-investigation/#preparing-boundary-linked-tabular-data) with exceptions:

-  [`spatial-profile`](https://discuss.okfn.org/t/geo-data-package/6143/26?u=stephen) applied at the resource level.
-  There is no `spatial-profile` for boundary-id data so added `"spatial-profile": "boundary-id"` so the data resource can be discovered as one containing location information

Note there is no service to resolve the location of the boundary data using `"codelist": "iso-3166-1:alpha-3"`.

## Data

This data is fictitious and should not be used for analysis

## License

The data is licensed under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).
