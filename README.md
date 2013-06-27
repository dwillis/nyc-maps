# NYC Maps

## Maps of New York City public geodata 

## Source

http://www.nyc.gov/html/dcp/html/bytes/applbyte.shtml
http://www.nyc.gov/html/dc/html/maps/maps.shtml

## Process

1. Navigate to http://www.nyc.gov/html/dcp/html/bytes/applbyte.shtml
2. Locate a dataset in the "ESRI Shapefile" format
3. Download the zip file
4. Use ogr2ogr to convert to `.geojson` with the `crs:84` SRS

## Bulk processing

1. Follow the steps above to download one or more zipped shapefiles
2. Run [this shell script](https://gist.github.com/benbalter/5858851)

## Requirements to convert

To convert shapefiles to geojson and reproject, you'll need [ogr2ogr](http://www.gdal.org/ogr2ogr.html). On OS X, the easiest way to do this is with [Homebrew](http://mxcl.github.io/homebrew/), by running the command `brew install gdal`.

## Contributing

1. Fork the project
2. Add a `.geojson` file
3. Submit a pull request

## Fine print

> The data made available here has been modified for use from its original source, which is the Government of New York City. The information contained in the BYTES of the BIG APPLE files was compiled for governmental use by the New York City Department of City Planning. The Department and the City make no representation as to the accuracy of the information or its suitability for any purpose. The Department and the City disclaim any liability for errors that may be contained therein.