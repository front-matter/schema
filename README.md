# DataCite Schema Repository

![Release](https://github.com/datacite/schema/workflows/Release/badge.svg)

This repository holds the official metadata schemas from DataCite as required
by the DataCite Metadata Store.

It contains the schemas itself along with examples and documentation.

## Schemas

Each schema has its own folder under `/source/meta`
e.g. `/source/meta/kernel-4/`. This directory is allowed to contain
only one xsd. The directory structure is as follow:

    /source/meta/{schema-name}/{filename}.xsd   root xsd
    /source/meta/{schema-name}/include/         referenced xsd files
    /source/meta/{schema-name}/example/         example xml files
    /source/meta/{schema-name}/doc/             documentation

The `/source/meta` directory will be published at http://schema.datacite.org, e.g.

    https://schema.datacite.org/meta/kernel-4/metadata.xsd

## Feedback

Learn more about contributing to the DataCite Metadata Schema here: [DataCite Schema - Contribute](https://schema.datacite.org/contribute.html).

## Tests

There are tests to check the directory structure, existence of examples,
validity of the schemas, and validity of the examples.

You can execute the tests via

```shell
rspec
```
