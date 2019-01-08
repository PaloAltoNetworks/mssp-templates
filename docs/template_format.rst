
Template Format
===============

The snippet directories are based on a common modeling including:

    + a metadata.yaml file

    + xml config snippets


The metadata.yaml file
----------------------

This file contains descriptive elements for loading the xml snippets using the Panorama or PAN-OS API.

Key elements of the metadata file include:

    + name: unique name descriptor specific to the directory contents

    + label: can be used by automation tools to create selection menus

    + description: what configuration content is contained in the directory

    + type: intended use by automation tools to determine API and commit models

    + extends: used to reference configurations to be loaded prior to this snippet

    + service_type: grouping label for automated selection menus

    + variables: variables used in the snippets include defaults and type if used by web utilities

    + snippets: ordered list of elements include the xml xpath and file pairing for API configuration


XML file snippets
-----------------
A complete set of xml elements to be loaded as part of the temmplate configuration.

    + any variables required must be added to the metadata.yaml file if used by configuration tools

    + the filenames are referenced in the snippets section of the metadata.yaml file


.. Note::
    For common xml snippets, relational references can be used to pull xml elements from other directories


