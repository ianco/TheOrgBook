[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

SonarQube Results:

[![Bugs](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook&metric=bugs&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook) [![Vulnerabilities](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook&metric=vulnerabilities&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook) [![Code smells](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook&metric=code_smells&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook) [![Coverage](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook&metric=coverage&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook) [![Duplication](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook&metric=duplicated_lines_density&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook) [![Lines of code](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook&metric=lines&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook) 

Zap Results:

[![Bugs](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook-Zap&metric=bugs&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook-Zap) [![Vulnerabilities](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook-Zap&metric=vulnerabilities&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook-Zap) [![Code smells](https://sonarqube.orgbook.gov.bc.ca/api/badges/measure?key=TheOrgBook-Zap&metric=code_smells&template=FLAT)](https://sonarqube.orgbook.gov.bc.ca/dashboard?id=TheOrgBook-Zap)

## TheOrgBook is now Aries Verifiable Credential Registry

[OrgBook BC](https://orgbook.gov.bc.ca) is a deployment of an underlying software component called a Verifiable Credential Registry (VCR). A VCR is more general component that can drive OrgBooks (repositories of information about registered organizations), and other repositories of verifiable information across a variety of use cases, including education, government services, public works projects and many more. The first generation of OrgBook BC was built on top of the software whose source code is in this repository. The current iteration of OrgBook BC is powered by the [Aries Verifiable Credential Registry (VCR)](https://github.com/bcgov/aries-vcr) (Aries VCR). TheOrgBook was implemented using custom protocols defined locally by the [Verifiable Organizations Network (VON)](https://vonx.io) team here in BC, Aries VCR is based on [Hyperledger Aries](https://www.hyperledger.org/use/aries) protocols defined by a global community at the [Linux Foundation](https://www.linuxfoundation.org/).

If you are interested in deploying your own OrgBook (perhaps for another jurisdiction), or learning about the internals of Verifiable Credential Registries, please start with the latest and greatest code in the [Aries VCR](https://github.com/bcgov/aries-vcr) open source repository.

If you are just interested in running the Greenlight demo to get a feel of how OrgBooks work at the user interface level, feel free to use this repository&mdash;instructions are below. We recommend that you don't build on top of the code in this repo.  Stick to [Aries VCR](https://github.com/bcgov/aries-vcr).

## TheOrgBook

TheOrgBook is a **Credential Registry** of verifiable credentials about entities. A public instance of TheOrgBook, such as [BC's OrgBook](https://orgbook.gov.bc.ca) contains a verifiable credentials about organizations (incorporations, professionals, etc.) issued by trusted public services such as Corporate Registries, regulatory agencies, permitting services, licencing services, procurement services and the like.

The Verifiable Organizations Network (VON) envisions the possibility of a number of public repositories of Verifiable Claims as a way of bootstrapping a trusted digital ecosystem.

`TheOrgBook` is being developed as part of the Verifiable Organizations Network (VON). For more information on VON see https://vonx.io.  Even, better - join in with what we are doing and contribute to VON and the Indy community.

## Quick Start Guide

The best way to get started with a new project is by working with a running instance.  The VON [Quick Start Guide](https://github.com/bcgov/greenlight/blob/master/docker/VONQuickStartGuide.md) will get you started with an [Indy Network](https://github.com/bcgov/von-network), an instance of [TheOrgBook (this repo)](https://github.com/bcgov/TheOrgBook) and an instance of [GreenLight](https://github.com/bcgov/greenlight) running on your local machine in Docker.  Give it a try!

OrgBook provides a set of RESTful web services you can use to query data from your third-party application, an introduction to use of these API's is available [here](docs/OrgBook-REST-Services.md).

## Running TheOrgBook on OpenShift

To deploy TheOrgBook on a local instance of OpenShift, refer to [Running TheOrgBook Locally on OpenShift](./RunningLocal.md).  These instructions, apart from the steps that are specific to setting up your local environment, can also be used to get the project deployed to a production OpenShift environment.

## Running TheOrgBook on Docker

The project can also be run locally using Docker and Docker Compose.  Refer to [Running TheOrgBook with Docker Compose](./docker/README.md) for instructions.

## Resetting the Ledger

For information on the process of resetting the ledger and wallets refer to the [Resetting the Ledger and Wallets](./ResettingTheLedger.md) documentation.