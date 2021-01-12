# Openware Versions

This repository is the only reliable source of latest Openware component versions.
It must be used during all deployments, e.g. by fetching `versions.yaml` and passing it to Helm.

## Usage

Every component's CI pipelines must have a step to update this repo whenever a new version is released.

Afterwards, this file could be fetched directly and passed to OpenDAX Helm or Compose without any changes.

## Structure

An example structure is:
```
opendax/
  2-6-stable/
    versions.yaml
  master/
    versions.yaml
great_product/
  1-0-stable/
    versions.yaml
```
