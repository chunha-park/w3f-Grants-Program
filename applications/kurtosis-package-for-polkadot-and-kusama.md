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
- [Docker](https://docs.docker.com/):
Docker is a software platform that allows you to build, test, and deploy applications quickly. Docker packages software into standardized units called containers that have everything the software needs to run including libraries, system tools, code, and runtime.

#### Supporting Implementations

- [D.I.V.E](https://github.com/HugoByte/DIVE): A powerful toolkit designed to streamline the entire process of node setup, network configurations, smart contract build and deployment currently supporting Ethereum, Cosmos and ICON ecosystems.
- [POC](https://github.com/HugoByte/PoCs/tree/master/polkadot-kurtosis-poc): A minimal kurtosis package able to deploy a single node of westend and local relay chain with single parachain.

#### Components

| Number | Component                                                                                          |
|--------|------------------------------------------------------------------------------------------------|
| 1      | Packages for Localnet, Testnet and Mainnet set up for Polkadot, Kusama and multiple parachains |
| 2      | Package for Chopstick                                                                          |
| 3      | Kurtosis provider for Zombienet                                                                |
| 4      | Explorer package                                                                               |
| 5      | Prometheus and Grafana package|                                                                               |

##### Chain List

| Number | Parachain      | Relay Chain | Image                                                        |
|--------|----------------|-------------|--------------------------------------------------------------|
| 1      | Acala          | Polkadot    | <https://hub.docker.com/r/acala/acala-node>                             |
| 2      | Ajuna Network  | Polkadot    | <https://hub.docker.com/r/ajuna/parachain-ajuna>             |
| 3      | Bifrost        | Polkadot    | <https://hub.docker.com/r/bifrostnetwork/bifrost>            |
| 4      | Centrifuge     | Polkadot    | <https://hub.docker.com/r/centrifugeio/centrifuge-chain>                      |
| 5      | Clover         | Polkadot    | <https://hub.docker.com/u/cloverio>                          |
| 6      | Frequency      | Polkadot    | <https://hub.docker.com/u/frequencychain>                    |
| 7      | Integritee Shell | Polkadot  | <https://hub.docker.com/r/integritee>                       |
| 8      | Interlay       | Polkadot    | <https://hub.docker.com/r/interlayhq/interbtc>               |
| 9      | KILT Spiritnet | Polkadot    | <https://hub.docker.com/r/kiltprotocol/mashnet-node>        |
| 10     | Kylin          | Polkadot    | <https://hub.docker.com/r/kylinnetworks/kylin-collator>     |
| 11     | Litentry       | Polkadot    | <https://hub.docker.com/r/litentry/litentry-parachain>      |
| 12     | Manta          | Polkadot    | <https://hub.docker.com/r/mantanetwork/manta>               |
| 13     | Moonbeam       | Polkadot    | <https://hub.docker.com/r/moonbeamfoundation/moonbeam>      |
| 14     | Moonsama       | Polkadot    | <https://hub.docker.com/r/moonsama/moonsama-node>           |
| 15     | Nodle          | Polkadot    | <https://hub.docker.com/r/nodlecode/chain>                  |
| 16     | Parallel       | Polkadot    | <https://hub.docker.com/u/parallelfinance>                   |
| 17     | Pendulum       | Polkadot    | <https://hub.docker.com/r/pendulumchain/pendulum-collator>  |
| 18     | Phala Network  | Polkadot    | <https://hub.docker.com/r/phalanetwork/phala-node>          |
| 19     | Polkadex       | Polkadot    | <https://hub.docker.com/r/polkadex/parachain>               |
| 20     | Subsocial      | Polkadot    | <https://hub.docker.com/r/dappforce/subsocial-parachain>    |
| 21     | Zeitgeist      | Polkadot    | <https://hub.docker.com/r/zeitgeistpm/zeitgeist-node>       |
| 22     | Encointer Network | Kusama   | <https://hub.docker.com/r/encointer/parachain>              |
| 23     | Altair         | Kusama      | <https://hub.docker.com/r/centrifugeio/centrifuge-chain>    |
| 24     | Bajun Network  | Kusama      | <https://hub.docker.com/r/ajuna/parachain-ajuna>            |
| 25     | Bifrost        | Kusama      | <https://hub.docker.com/r/bifrostnetwork/bifrost>           |
| 26     | Calamari       | Kusama      | <https://hub.docker.com/r/mantanetwork/calamari>            |
| 27     | Karura         | Kusama      | <https://hub.docker.com/r/acala/karura-node>                |
| 28     | Khala Network  | Kusama      | <https://hub.docker.com/r/phalanetwork/khala-node>          |
| 29     | Kintsugi BTC   | Kusama      | <https://hub.docker.com/r/interlayhq/interbtc>              |
| 30     | Litmus         | Kusama      | <https://hub.docker.com/r/litentry/litentry-parachain>      |
| 31     | Mangata        | Kusama      | <https://hub.docker.com/r/mangatasolutions/mangata-node>    |
| 32     | Moonriver      | Kusama      | <https://hub.docker.com/r/moonbeamfoundation/moonbeam>      |
| 33     | Robonomics      | Kusama      | <https://hub.docker.com/r/robonomics/robonomics>            |
| 34     | subzero        | Kusama      | <https://hub.docker.com/r/playzero/subzero>                 |
| 35     | Turing Network | Kusama      | <https://hub.docker.com/r/oaknetwork/turing>                |

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
- Shanith K K (System Developer)
- Abhishek Harde (System Developer)
- Hemanth Kumar (Senior Tester)
- Principal Engineer

### Contact

- **Contact Name:** Muhammed Irfan K
- **Contact Email:** <muhammedirfan@hugobyte.com>
- **Website:** <https://hugobyte.com>

### Legal Structure

- **Registered Address:** Business Center 1, M Floor The Meydan Hotel, Nad Al Sheba, Dubai, United Arab Emirates
- **Registered Legal Entity:** HUGOBYTE NETWORK LABS L.L.C-FZ, Trade License Number: 2305566.01

### Team's experience

HugoByte is the go-to expert for all things Web 3.0. We specialize in creating tools and solutions that simplify Web 3.0 development and bring it closer to reality.

Our Key Products:

1. **DIVE - One-Click Deployment:** DIVE is a user-friendly tool that makes it incredibly easy to set up nodes, bridges, and contracts for your blockchain projects. It's like the "easy" button for Web 3.0. Plus, it supports cross-chain development, ensuring your projects can work seamlessly on different blockchains.

2. **Aurras - Notifications and Automation:** Aurras a low-code workflow orchestration platform that is decentralized systems. It's perfect for projects that need to keep everyone in the loop, with support for cross-chain notifications and automated payouts on Polkadot.

Our Principles:

- **Open Source Advocacy:** We believe in sharing and collaboration. Our code is open source, which means community can access it and contribute to its growth.

- **Interoperability Experts:** We're all about making different blockchains work together. Our solutions are built with interoperability in mind, ensuring all projects can communicate with multiple networks effortlessly.

- **Web 3.0 Innovators:** We're always on the cutting edge, pushing the boundaries of what's possible in the Web 3.0 world. Our team is committed to making the decentralized future a reality.

HugoByte is here to simplify the Web 3.0 journey. We provide user-friendly tools and solutions, follow open source principles, and excel at making different blockchains work together.

- **Muhammed Irfan - CEO**
As a Solutions architect and CEO at HugoByte Network Labs with 10+ years of invaluable industry experience, Muhammed Irfan possesses exceptional expertise in multiple domains such as Web3, Blockchain, Interoperability Solutions, Enterprise, Infrastructure and AI. He is also highly proficient in designing state-of-the-art architecture and infrastructure, as well as mastering full-stack development.

- **Shreyas K S - Senior Developer**
He has 5 years of professional experience, Shreyas currently serves as the Development Tech Lead with the designation of Senior Systems Developer at HugoByte as a core developer and Tech Lead, Shreyas played a pivotal role in the rollout of the kurtosis package for Icon, ETH, hardhat, and BTP. His extensive contributions to open-source communities are notably highlighted by his significant involvement in projects like ICON IBC-Integration and DIVE.
Skill-wise, Shreyas is proficient in Rust, Golang, Python, and Starlark. His technological expertise encompasses Blockchain, Smart Contract Development, Workflow Orchestration, and Database Management. Shreyas possesses a deep understanding of blockchain, smart contracts, and is adept in various workflow orchestration tools. His experiences have shaped him into a collaborative team player and a decisive leader, known for consistently guiding projects to successful completion. Driven by a passion to employ technology in solving intricate problems, Shreyas remains eager to contribute further to the dynamic world of tech.

- **Abhishek Harde - System Developer**
He is a system developer with over two years of experience in creating reliable and scalable software solutions using Rust, GoLang, Starlark, C#, and C++. As a part of HugoByte, he majorly contributes to the DIVE project development. He has also implemented the kurtosis package for setting up nodes for Archway, Neutron, and IBC relay. Previously, he has experience as a .NET core developer, where he developed web applications and APIs using ASP.NET Core, Entity Framework Core, and Azure. He is passionate about blockchain technology and its applications in various domains. He is always eager to learn new technologies and tools that can improve his skills and knowledge.

- **Shanith K K - System Developer**
He is a system developer with over 2+ years of experience in programming languages such as Rust, Python, Starlark, and JavaScript. He has handled innovative projects like Aurras and D.I.V.E at HugoByte. He has also gained valuable experience working with the Polkadot ecosystem and exploring various blockchains like NEAR and ICON. He enjoys mentoring junior developers to achieve excellent outcomes, contributing to the growth and development of the team. With his contribution as the primary developer, HugoByte won the xCall incentive program conducted by ICON and also worked as a focus tester for the xCall focus tester program. These experiences have provided him with a deep understanding of the ICON ecosystem and made him a respected DAO Iconist. His passion for development fuels his continuous learning of new technologies and advancements in the field, ensuring that he stays up-to-date with industry trends and best practices, ultimately resulting in high-quality outcomes.

- **Hemanth Kumar - Senior Tester**
He is a senior tester with more than nine years of dedicated experience, specializing in the intricate realms of automation, end-to-end (E2E), manual, and integration testing. One of his notable accomplishments includes the development of a customized E2E testing framework tailored to the exacting requirements of IBC message transfers across a diverse array of blockchain ecosystems. This innovation ensures the seamless and uninterrupted flow of critical data between blockchain networks. With a well-documented track record in scrutinizing smart contracts on multiple blockchain platforms, he exhibits a consummate command of programming languages such as Python, Golang, and Typescript, thus enhancing the finesse of test automation and development. His proficiency also extends to writing automation testing scripts for GitHub, which underpins his commitment to streamlined processes and the unwavering pursuit of code quality. Beyond these technical achievements, his considerable exposure to the intricacies of the Polkadot ecosystem further underscores his commitment to the dynamic field of blockchain testing and the pursuit of seamless interoperability strategies.

Previously funded Web3 Foundation grant:

- Aurras MVP  
  HugoByte AI Labs Private limited

### Team Code Repos

- <https://github.com/HugoByte>
- <https://github.com/HugoByte/DIVE>
- <https://github.com/HugoByte?q=aurras>
- <https://github.com/MuhammedIrfan>
- <https://github.com/Mr-Nobody21>
- <https://github.com/shreyasbhat0>
- <https://github.com/shanithkk>
- <https://github.com/abhiyana>
- <https://github.com/hemz10>

### Team LinkedIn Profiles

- <https://www.linkedin.com/in/muhammed-irfan-k/>
- <https://www.linkedin.com/in/siddh-jain/>
- <https://www.linkedin.com/in/shreyas-ks/>
- <https://www.linkedin.com/in/shanith-k-k-09378988/>
- <https://www.linkedin.com/in/abhishek-harde-056a2a1a8/>
- <https://www.linkedin.com/in/the-hemanth-profile/>

## Development Status :open_book:

- This package is component of a broader project which aims to offer vercel like deployment experience for Collators, Parachains and Validators which is in discussion with [Santiago Balaguer](https://github.com/SBalaguer).
- [POC](https://github.com/HugoByte/PoCs/tree/master/polkadot-kurtosis-poc)

## Development Roadmap :nut_and_bolt:

### Milestone Overview

- **Total Estimated Duration:** 9-10 weeks
- **Full-Time Equivalent (FTE):** 3
- **Total Costs:** 46,000 USD

### Milestone 1 — Kurtosis Package for Localnet, Testnet and Mainnet setup

- **Estimated duration:** 4 weeks
- **FTE:** 3 (System Engineer (2) + Project Manger (0.5) + Lead Developer (0.5))
- **Costs:** 18,000 USD

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

### Milestone 2  — Kurtosis Package for chopstick, Explorer, Prometheus, Grafana and Integration with Zombienet

- **Estimated duration:** 3 weeks
- **FTE:** 3.5 (Principle Engineer (1) + System Engineer (1) + Project Manger (0.5) + Tester (1))
- **Costs:** 19,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 |
| **0b.** | Documentation | We will provide the following documentation: Inline Code Documentation, Readme.md file, Configuration Documentation, Usage Documentation |
| **0c.** | Testing and Testing Guide | We will compose a testing guide to describe how to run tests. The code will have unit-test coverage (min. 50%) to ensure functionality and robustness |
| **0d.** | Docker | N/A as this is a package definition which will be executed through Kurtosis CLI |
| 1. | Package for Chopstick | This package contains definitions to deploy chopstick |
| 2. | Kurtosis provider for Zombienet | This will be created as PR to enable to use Kurtosis as one of the provider to use above packages for deployment |
| 3. | Test Script for message testing | This will be robust test script to run automated test using the above packages |
| 4. | Explorer deployment package | This contains package definitions for deploying Polkadot.JS Explorer |
| 5. | Prometheus and Grafana package | This package will include Prometheus and Grafana package for Metrics and observability |

### Milestone 3  — R&D for Bridge, One click Node deployment and Custom Parachain build package

- **Estimated duration:** 2 weeks
- **FTE:** 1.5 (Principle Engineer (1) + Project Manager (0.5) )
- **Costs:** 9,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 |
| **0b.** | Documentation | We will provide document for the Research performed |
| **0c.** | Testing and Testing Guide | N/A |
| **0d.** | Docker | N/A |
| **0e.** | Article | We will write a Medium article that explains the work done as part of the grant |
| 1. | R&D for Bridge Setup |  Research and Documentation for packages for bridge setup |
| 2. | R&D for One click Node deployment | Research and Documentation to enable one click deployment for Collators, Parachains and Validators |
| 3. | R&D for Custom Parachain build package | Research and Documentation to create a build package to build images for parachains by injecting the binaries |

## Future Plans

- Enable deployment of custom collator and parachains.
- Enable Vercel like deployment experience.
- Enable deployment for Bridges.
- Integrate the packages to DIVE.
