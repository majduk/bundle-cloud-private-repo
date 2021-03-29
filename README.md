# Basic OpenStack Cloud Repository

This bundle deploys a private local mirror with all the dependencies needed to build Charmed Openstack Ussuri on Ubuntu Bionic with Juju and MAAS.

## Requirements

Single server meeting:

 - A minimum of 12GB of physical RAM.
 - Enough CPU cores to support your capacity requirements.
 - At least 300GB of available storage


## Components

 - 1 LXD container exposing APT packages, MAAS, Juju and LXD images.
 - 1 LXD container exposing Snap Proxy

## Deployment

With a Juju controller bootstrapped on a MAAS cloud with no network spaces
defined, a basic non-HA cloud can be deployed with the following command:

    juju deploy bundle.yaml

