# PostgreSQL Client Containers

These images extract the postgres client tools out of the official postgres alpine
images in order to minimise as much as possible.

## Thanks

With thanks to:

- [tensorchord/cloudnative-pgvecto.rs](https://github.com/tensorchord/cloudnative-pgvecto.rs)
  for the inspiration for using renovate and the basics of the github workflow found in
  this repository.

## Building

To build the Dockerfile locally, you need to pass the CNPG_TAG, DISTRO and PG_REPACK_TAG args. 

For example:
`docker build . --build-arg="PG_VERSION=16.9" --build-arg="ALPINE_VERSION=3.22"`
