# WordPress Harvester

CLI app for harvesting content from WordPress via its REST API.

## Using this tool

This section describes how to use this tool for its intended purpose. TBD.

At the moment, I'm thinking that the ideal command will end up being something
like:
```
pipenv run wordpress_harvester -h https://libraries.mit.edu/ -e pages -e posts -e experts -e locations
```

## Development

- To install with dev dependencies: `make install`
- To update dependencies: `make update`
- To run unit tests: `make test`
- To lint the repo: `make lint`
- To run the app: `pipenv run wordpress_harvester --help`

## Required ENV

- `SENTRY_DSN` = If set to a valid Sentry DSN, enables Sentry exception monitoring. This is not needed for local development.
- `WORKSPACE` = Set to `dev` for local development, this will be set to `stage` and `prod` in those environments by Terraform.
