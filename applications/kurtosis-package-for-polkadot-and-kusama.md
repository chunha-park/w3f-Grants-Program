# Kurtosis Package for Polkadot and Kusama

- **Team Name:** HugoByte Network labs LLC-FZ
- **Payment Address:** ETH (USDC) 0x3de51De78742De3a7aD4F65ae0B508535dA22489
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 3


## Project Overview :page_facing_up:

### Overview

This project aims to implement environment definitions through [Kurtosis package](https://docs.kurtosis.com/concepts-reference/packages) for Polkadot and Kusama. The Kurtosis services and API are designed to simplify the process of deploying various nodes and services in development, testing and production environments eliminating complicated steps and minimizing dependencies. This package will serve as a one stop solution for all the node deployments across the substrate ecosystem. It will be capable of setting up nodes, development and testing utilities, such as chopstick and zombienet, explorers, and can be extended to support bridges.

### Project Details

#### Technologies
- [Kurtosis](https://docs.kurtosis.com/): Kurtosis is a platform for packaging and launching environments of containerized services ("distributed applications") with a focus on approachability for the average developer. What Docker did for shipping binaries, Kurtosis aims to do even better for distributed applications.
- [Starlark](https://docs.kurtosis.com/starlark-reference): Starlark is a dialect of Python intended for use as a configuration language. Starlark is used as DSL for creating environment definitions in Kurtosis which helps in sharing and reusing distributed application components.

#### Supporting Implementations
- [D.I.V.E](https://github.com/HugoByte/DIVE): A powerful utility designed to streamline the entire process of node setup, network configurations, smart contract build and deployment currently supporting Ethereum, Cosmos and ICON.
- [POC](https://github.com/HugoByte/PoCs/tree/master/polkadot-kurtosis-poc): A minimal kurtosis package able to deploy a single node of westend and local ralay chain with single parachain.

#### Components

| Sr. No | Items                                                                                          |
|--------|------------------------------------------------------------------------------------------------|
| 1      | Packages for Localnet, Testnet and Mainnet set up for Polkadot, Kusama and multiple parachains |
| 2      | Package for Chopstick                                                                          |
| 3      | Kurtosis provider for Zombienet                                                                |
| 4      | Explorer package                                                                               |


### Ecosystem Fit

With the impending core changes in Coretime, extensive testing and multiple re-deployments will be essential. This project's primary objective is to create a comprehensive deployment solution for the Polkadot and Kusama ecosystems.

This package is set to usher in a paradigm shift in parachain development. One of its standout features is its capability to create new parachains through the simple authoring of a basic configuration file. Moreover, it will not be limited to deploying just the relay chain for Polkadot and Kusama, but will also support the deployment of parachains.

This versatile package will cater to a range of node types, including validator nodes, RPC nodes, collator nodes, and archival nodes. It will further offer deployment options for both cloud and local environments, ensuring flexibility and convenience.

Kurtosis is a multi-container system that simplifies the deployment process and enables the running of multiple blockchain nodes. This feature significantly reduces the amount of time and effort required to set up nodes individually and makes the deployment process more efficient.

Moreover, the dynamic setup of nodes can be a source of errors. For instance, passing IPs or runtime-generated data between services or contracts can lead to errors during the setup. Kurtosis eliminates these issues, making the deployment process more reliable and error-free.

By implementing Kurtosis, errors during deployment can be reduced, and it becomes easier to set up environments for development and testing purposes. It streamlines the entire process, allowing developers to focus on other essential tasks and enhancing the overall user experience.

#### Why use Kurtosis?
Developers usually set up dynamic environments with a free-form scripting language like bash or Python, interacting with the Docker CLI or Docker Compose. Kurtosis is designed to make these setups easier to maintain and reuse in different test scenarios.

In Kurtosis, test environments have these properties:

- Environment-level portability: the entire test environment always runs the same way, regardless of the host machine.  
- Composability: environments can be composed and connected without needing to know the inner details of each setup.  
- Parameterizability: environments can be parameterized, so that they’re easy to modify for use across different test scenarios.    

Kurtosis aims to bring DevOps back, by providing the developer with a single platform for prototyping, testing, debugging, deploying to Prod, and observing the live system.

## Team :busts_in_silhouette:

### Team members

- Muhammed Irfan K (Leader)
- Siddh Jain (Project Manager)
- Shreyas K S (Lead Developer)
- Shanith K K (Developer)
- Abhishek Harde (Developer)
- Hemanth Kumar (Senior Tester)

### Contact

- **Contact Name:** Muhammed Irfan K
- **Contact Email:** muhammedirfan@hugobyte.com
- **Website:** https://hugobyte.com

### Legal Structure

- **Registered Address:** Business Center 1, M Floor The Meydan Hotel, Nad Al Sheba, Dubai, United Arab Emirates
- **Registered Legal Entity:** HUGOBYTE NETWORK LABS L.L.C-FZ, Trade License Number: 2305566.01

### Team's experience

HugoByte is deeply rooted in the Web 3 domain with strong experience in creating bridges and web 3 development utilities.

Previously funded Web3 Foundation grant:
- Aurras MVP  
  HugoByte AI Labs Private limited

### Team Code Repos

- https://github.com/HugoByte
- https://github.com/HugoByte/DIVE
- https://github.com/HugoByte?q=aurras


Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/MuhammedIrfan
- https://github.com/Mr-Nobody21
- https://github.com/shreyasbhat0
- https://github.com/shanithkk
- https://github.com/abhiyana
- https://github.com/hemz10


### Team LinkedIn Profiles

- https://www.linkedin.com/<person_1>
- https://www.linkedin.com/<person_2>


## Development Status :open_book:

- This package is component of a broader project which aims to offer vercel like deployment experience for Collators, Parachains and Validators which is in discussion with [Santiago Balaguer](https://github.com/SBalaguer).
- [POC](https://github.com/HugoByte/PoCs/tree/master/polkadot-kurtosis-poc)

## Development Roadmap :nut_and_bolt:

### Overview

- **Total Estimated Duration:** 2-3 Months
- **Full-Time Equivalent (FTE):** 3.5 FTE
- **Total Costs:** 

### Milestone 1 — Kurtosis Package for Localnet, Testnet and Mainnet setup

- **Estimated duration:** 1.5 month
- **FTE:**  2.5
- **Costs:** 


| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can spin up different type of nodes. |
| **0c.** | Testing and Testing Guide | We will provide users guide on how users can perform dry run to ensure packages are out of syntax errors. |
| **0d.** | Docker | N/A as this is a package definition which will be executed through Kurtosis CLI |
| 1. | Relay chain package |  This package contains definitions for deploying the Polkadot and Kusama relay chain. |
| 2. | Validator Node package | This package contains definitions for deploying Validator Nodes. |
| 3. | RPC Node package | This package contains definitions for deploying RPC Nodes. |
| 4. | Collator Node package | This package contains definitions for deploying Collator Nodes. |
| 5. | Parachain package | This package contains definitions for deploying specified parachains. |
| 6. | Parachain Network Setup (Relay + Parachain + Validator + RPC + Collator Node) | This configuration targets to create a full fledge Parachain network. |


### Milestone 2  — Kurtosis Package for chopstick, Explorer and Integration with Zombienet 

- **Estimated duration:** 1.5 month
- **FTE:**  3.5
- **Costs:** 


| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 |
| **0b.** | Documentation | We will provide the following documentation: Inline Code Documentation, Readme file, Configuration Documentation, Usage Documentation |
| **0c.** | Testing and Testing Guide | We will compose a testing guide to describe how to run tests. The code will have unit-test coverage (min. 50%) to ensure functionality and robustness |
| **0d.** | Docker | N/A as this is a package definition which will be executed through Kurtosis CLI |
| 1. | Package for Chopstick | This package contains definitions to deploy chopstick |
| 2. | Kurtosis provider for Zombienet | This will be created as PR to enable to use Kurtosis as one of the provider to use above packages for deployment |
| 3. | Test Script for message testing | This will be robust test script to run automated test using the above packages |
| 4. | Explorer deployment package | This contains package definitions for deploying Polkadot.JS Explorer |
| 5. | R&D for Custom Parachain build package | Research and Documentation to create a build package to build images for parachains by injecting the binaries | 

### Milestone 3  — R&D for Bridge and One click Node deployment 

- **Estimated duration:** 0.5 month
- **FTE:**  3
- **Costs:** 

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 |
| **0b.** | Documentation | We will provide document for the Research performed |
| **0c.** | Testing and Testing Guide | N/A |
| **0e.** | Article | We will write a Medium article that explains the work done as part of the grant |
| 1. | R&D for Bridge Setup |  Research and Documentation for packages for bridge setup |
| 2. | R&D for One click Node deployment | Research and Documentation to enable one click deployment for Collators, Parachains and Validators |

## Future Plans

- Enable deployment of custom collator and parachains.
- Enable Vercel like deployment experience.
- Enable deployment for Bridges.
- Integrate the packages to DIVE.