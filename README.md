# Represent Postcodes

[Represent](https://represent.opennorth.ca/) is the open database of Canadian elected officials and electoral districts. It provides a [REST API](https://represent.opennorth.ca/api/) to boundary, representative, and postcode resources.

This repository provides an API to postal codes. API documentation is available at [represent.opennorth.ca/api/](https://represent.opennorth.ca/api/#postcode).

The [represent-canada](https://github.com/opennorth/represent-canada) repository provides a master Django project, and points to packages which add boundary, representative, and map features.

## Adding data

Load postal code centroids with:

    python manage.py loadpostcodes data/shapefiles/postcodes/ocd-division/country:ca/Canada.csv

Load postal code concordances with:

    python manage.py loadpostcodeconcordance --help

## Bugs? Questions?

Please submit bug reports, feature requests, and feedback to [represent-canada](https://github.com/opennorth/represent-canada).

Released under the MIT license
