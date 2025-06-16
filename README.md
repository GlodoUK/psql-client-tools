# PostgreSQL Client Containers

These images extract the postgres client tools out of the official postgres alpine
images in order to minimise as much as possible.

## Thanks

With thanks to:

- [tensorchord/cloudnative-pgvecto.rs](https://github.com/tensorchord/cloudnative-pgvecto.rs)
  for the inspiration for using renovate and the basics of the github workflow found in
  this repository.
- renovate for the automated updating.

## Building

To build the Dockerfile locally:
`docker build . --build-arg="PG_VERSION=16.9" --build-arg="ALPINE_VERSION=3.22"`
