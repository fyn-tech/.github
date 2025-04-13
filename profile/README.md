# Fyn-Tech

Note: This project is still in the very early stages of development, so it's rough around many edges, and most things are likely to change.

## Background

The objective of the project is to build, from the ground up, a cloud-based CFD solver. The front end will be browser-based; you can view a very simple 'mock up' [here](https://fyn-tech.com/). 
Using the web browser, a user will be able to set up a CFD simulation and then run it either locally or in the cloud, with the compute resources and job management in the web interface.

The name Fyn-Tech is short for Fynbos Technology, where [Fynbos](https://en.wikipedia.org/wiki/Fynbos) is a unique biome in the southwestern region of South Africa.

## Organisation

The project is split into several different repositories, with the CFD solver code not yet made public. 
- [fyn-env](https://github.com/fyn-tech/fyn-env) The Fyn-Tech repository for managing and coordinating deployments across all other repos.
- [fyn-front](https://github.com/fyn-tech/fyn-front) The front-end repository, Rust conversation under consideration.
- [fyn-front](https://github.com/fyn-tech/fyn-front) The front-end repository, Rust conversation under consideration.
- [fyn-api](https://github.com/fyn-tech/fyn-api) The back-end AWS hosted Django backend.
- [fyn-runner](https://github.com/fyn-tech/fyn-runner) The runner for CFD simulation job execution on remote resources.
- [fyn-schema](https://github.com/fyn-tech/fyn-schema) Protobuf repository for consistent communication accoss applications.
- [Disa](https://github.com/bevanwsjones/Disa), ultimately the 'native' linear algebra function.

## Current Focus

The current focus of the project is to set up a 'MVP' of sorts where a simple geometry can be uploaded and an incompressible simulation configured from the front end.
Once completed, it should be submitted to the backend and executed on a connected remote resource (initially a local machine using the runner). 
This will also require a functional runner-backend system, which is currently the development focus. 
