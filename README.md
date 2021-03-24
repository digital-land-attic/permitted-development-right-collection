# permitted-development-right collection

[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/digital-land/brownfield-land/blob/master/LICENSE)

A collection of permitted-development-right categories and types.

The national dataset is in a format consistent with other Digital Land datasets as defined by the following schemas:

* [permitted-development-right](https://digital-land.github.io/specification/schema/permitted-development-right/)
* [permitted-development-right-class](https://digital-land.github.io/specification/schema/permitted-development-right-class/)
* [permitted-development-right-part](https://digital-land.github.io/specification/schema/permitted-development-right-part/)

# Collection

* [collection/source.csv](collection/source.csv) — the list of data sources by organisation, see [specification/source](https://digital-land.github.io/specification/schema/source/)
* [collection/endpoint.csv](collection/endpoint.csv) — the list of endpoint URLs for the collection, see [specification/endpoint](https://digital-land.github.io/specification/schema/endpoint)
* [collection/resource/](collection/resource/) — collected resources
* [collection/log/](collection/log/) — individual log JSON files, created by the collection process
* [collection/log.csv](collection/log.csv) — a collection log assembled from the individual log files, see [specification/log](https://digital-land.github.io/specification/schema/log)
* [collection/resource.csv](collection/resource.csv) — a list of collected resources, see [specification/resource](https://digital-land.github.io/specification/schema/resource)

# Updating the collection

We recommend working in [virtual environment](http://docs.python-guide.org/en/latest/dev/virtualenvs/) before installing the python [requirements](requirements.txt), [makerules](https://github.com/digital-land/makerules) and other dependencies. Requires Make v4.0 or above.

    $ make makerules
    $ make init
    $ make collect

# Updating the collection

This collection is maintained manually by editing the files in the [data](data) directory.
The collected files can then be converted into a national dataset:

    $ make

# Licence

The software in this project is open source and covered by the [LICENSE](LICENSE) file.

Individual datasets copied into this repository may have specific copyright and licensing, otherwise all content and data in this repository is
[© Crown copyright](http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/copyright-and-re-use/crown-copyright/)
and available under the terms of the [Open Government 3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) licence.
