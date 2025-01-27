
## 0.3.0 (2021-09-10)

* Move `raster:bands` information in assets (not in properties).
* update pystac version
* fix typo for `stddev` raster information
* drop support of python 3.6 (pystac 1.0.0 dropped support of python 3.6)

## 0.2.1 (2021-08-24)

* use WarpedVRT for data with internal GCPS

## 0.2.0 (2021-07-06)

* fix validation issue with Collection and extension for STAC 1.0.0
* add collection_url option to customize the collection link
* add `raster` extension option (https://github.com/developmentseed/rio-stac/pull/12)
* set `proj:epsg` value to `None` when no `CRS` is found in the dataset.

**breaking changes**

* update pystac version to `>=1.0.0rc1`
* use full URL for extension
* add Collection Link when adding a collection
* add with_proj (--with-proj/--without-proj in the CLI) in `create_stac_item` to add the extension and proj properties in the stac items (will do the same for the raster extension)

## 0.1.1 (2021-03-19)

* fix CLI asset-href default

## 0.1.0 (2021-03-19)

Initial release.

* Design API
* add CLI
* add tests
* write docs
