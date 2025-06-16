<!--
SPDX-FileCopyrightText: 2025 Deutsche Telekom AG

SPDX-License-Identifier: CC0-1.0    
-->

# Open Telekom Integration Platform

<p align="center">
    <img src="img/Open-Telekom-Integration-Platform_Visual.svg" alt="Visual" width="200">
</p>

## About

The Open Telekom Integration Platform is a complete and integrated suite of distributed, cloud-native and cloud-agnostic
components for synchronous APIs, asynchronous messaging patterns and file transfer. It is an integral part of Telekom's
architecture strategy.

The platform is modular in nature. It is currently in an early release stage. Thus, the key components are already
available with many more to follow.

**This repository contains the overarching documentation.**

For the actual code, an overview of the available repositories is available
here: [Repositories](docs/repository_overview.md).

## Code of Conduct

This project has adopted the [Contributor Covenant](https://www.contributor-covenant.org/) in version 2.1 as our code of
conduct. Please see the details in our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). All contributors must abide by the code
of conduct.

By participating in this project, you agree to abide by its [Code of Conduct](./CODE_OF_CONDUCT.md) at all times.

## Licensing

This project follows the [REUSE standard for software licensing](https://reuse.software/).
Each file contains copyright and license information, and license texts can be found in the [./LICENSES](./LICENSES)
folder. For more information visit https://reuse.software/.

## Getting Started

A comprehensive guide on how to get started with the installation of the Open Telekom Integration Platform is available
here: [Getting Started](https://github.com/telekom/Open-Telekom-Integration-Platform/wiki/Getting-Started).

### How to Build

We provide build scripts for the Open Telekom Integration Platform components. The build scripts are meant to be a starting
point for your own build scripts. Please see the [build](./build) directory for more information.

## In A Nutshell

### High-Level Architecture

The picture below shows the high-level architecture of the Open Telekom Integration Platform. Further, it indicates the
progress of open-sourcing the platform's components.

![High-Level Architecture](./img/Open-Telekom-Integration-Platform_High-Level-Architecture.svg)

### Principles

| Decoupling Done Right                                                                                                                                                                                                                                                                         | Custom Open Source                                                                                                                    | Secure By Design                                                                                                                      |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| The Open Telekom Integration Platform's fundamentals are cloud-centric and API-first. It is a complete and integrated suite of distributed, cloud-native and cloud-agnostic components for synchronous APIs and asynchronous messaging patterns. It is designed to be deployed on Kubernetes. | It is built based on top of open-source software, with all custom extensions capsuled in separate modules to remain product agnostic. | It provides secure and auditable access to APIs, with features like 4-eyes-principle, approval expiration, recertification, and more. |

### Paradigms

| Declarative Configuration                                                                                                                                                                                                                                                                                             | Pipeline-Driven                                                                                                                                                                                            | Self-Service                                                                                                                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| The Open Telekom Integration Platform is configured declaratively, using YAML files. This allows for easy versioning, and the ability to use tools like Git to manage the configuration. You are just defining the desired state of the system, and the configuration tool (namely Rover) will take care of the rest. | Rover can run in a CICD-pipeline and is designed for that purpose. It enables the configuration to be integrated into a CICD-pipeline alongside the application code, and to be deployed together with it. | The Open Telekom Integration Platform is designed to be used by developers and operators alike. It provides a self-service eliminating the need for a central middleman. |

### Core Capabilities

| API Management                                                                                                                                                                                                                                                                                                 | Event-Driven Integration (Pub/Sub)                                                                                                                                                                                                                                                                        | 
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| The Open Telekom Integration Platform supports the whole API lifecycle and allows seamless, cloud-independent integration of services. Further, it enables a fine-grained and vigilant API access control. The communication is secure by design, utilizing OAuth 2.0 and an integrated permission management. | The Open Telekom Integration Platform offers a component for asynchronous communication of services. It focuses on a resilient and loss-free event delivery, while maintaining high throughput volumes. Advanced filtering, payload validation and conditional delivery are also part of the feature set. |
