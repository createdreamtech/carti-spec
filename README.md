# Carti Spec
Carti - general specification for a Cartesi machine package system
### Overview
This repo contains the specification for package system for Cartesi. It includes the specification for what makes a repository service that hosts Carti packages, as well as the package description schema itself.

### Carti Package Schema - carti_pacakge_schema.json
This represents the spec that is used to describe a Carti package, in JSON schema format. The ultimate storage format will be using IPLD. This is just a place holder until I add an IPLD schema representation. The schema.json contains all the same logical elements as the IPLD. JSONSchema is more well known so this will probably stay in place for a long time to help developers get familar wit the fields you can check this out [here](http://nowhere yet)

### Carti Repository Service Schema - openrpc.json
This represents what makes a carti repository service. It is written in [OpenRPC](https://open-rpc.org) a JsonRPC description language. This was done to make it easy to generate clients to connect to services as well as provide implementers with ways to generate custom server [scaffolding](https://github.com/open-rpc/generator)( directly from the schema description. 

### Motivation
The idea behind Carti Spec is to make an open description of how to package Cartesi machines. Decoupling the implementations from the specs will allow for many different implementors to pick up the mantle and develop against Carti and build tooling around it. The aim is to improve the state of Cartesi machine sharing with increased meta data and good tooling.

