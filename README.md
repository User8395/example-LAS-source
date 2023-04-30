# Example LAS source
An example source for LAS

## NOTE
As LAS is still a pre-alpha, this repository may not work in earlier stages of development. Information here is subject to change.

## About
To install apps, LAS gets data from different "sources", which are just Git repositories.

Every source contains a folder with `.lapp` files. These are compressed files containing the app and it's data, which are extracted to `~/.las/apps/`.

The root of the source contains 2 JSON files, `sources.json`, and `apps.json`.

### `info.json`
This file contains basic source information.

### `apps.json`
This file contains a list of every app and where they can be downloaded from.

If the `url` is set to `auto`, LAS will then automatically download the app from `/apps/app.lapp`, `/` being the root of the source.

## Making your own source
TODO