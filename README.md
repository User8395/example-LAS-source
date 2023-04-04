# Example LAS source
An example source for LAS

## NOTE
As LAS is still a pre-alpha, this repository may not work in earlier stages of development. Information here is subject to change.

## About
To install apps, LAS gets data from different "sources", which are  just Git repositories.

LAS uses two types of repositories:

1. Informatory Repositories (short: info-repo), used to provide info about a specific source.
2. Application Repositories (short: app-repo), contains a single app.

## Info repos

Info-repos are used to provide information about an repository and it's apps. Every info-repo needs these files:

```
├─ info.json
└─ apps.json
```
`info.json` contains information about the repository, and `apps.json` contains the apps themselves and where they can be downloaded from.

Example `info.json`:

```
{
    "type": "info",
    "name": "Example LAS Source",
    "description": "An example source for LAS"
}
```
|    Property     |       Description      | Allowed values |
|-----------------|------------------------|----------------|
|     `type`      |     Repository type    |  `info`, `app` |
|     `name`      |     Repository name    |      any       |
|  `description`  | Repository description |      any       |
|    `version`    |    Repository version  |       1        |



Example `apps.json`

```
{
    "hello-world": "na"
}
```
|    Property     |                                  Description                                    | Allowed values |
|-----------------|---------------------------------------------------------------------------------|----------------|
|  `hello-world`  | Title must contain app name and value must contain link to app's Git repository |      any       |



## TODO
Incomplete, finishing later on