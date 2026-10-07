# Awesome-IoT-Cloud-Connectivity-Messaging

## Top IoT Cloud Connectivity & Messaging Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on MQTT Brokers, Device Connectivity & Self-Hosted IoT Messaging*  

**Last updated: October 2026**



This repository tracks notable **commercial IoT cloud connectivity platforms** and **open-source projects** that connect devices to the cloud, route telemetry, and enable bidirectional messaging at scale — from managed MQTT brokers to self-hosted IoT messaging backbones with fine-grained access control.



**Examples** include AWS IoT Core, Azure IoT Hub, Google Cloud IoT, Particle, EMQX Cloud, HiveMQ Cloud, Losant, ThingsBoard, Ayla Networks, and Kaa IoT (the category leaders).



**Open-source emphasis**: IoT cloud connectivity is one of the strongest open-source domains. **EMQX** leads as the most scalable MQTT broker with 100M+ connection support and 13,000+ GitHub stars . **Mosquitto** remains the reference lightweight MQTT broker with 8,000+ stars . **NanoMQ** brings ultra-lightweight MQTT to edge gateways with 1.7MB binary size . **VerneMQ** delivers distributed clustering for mission-critical deployments . **HiveMQ Community Edition** provides enterprise-grade MQTT semantics with an open-source core . **Magistrala** offers a Go-based, cloud-native IoT platform with fine-grained access control and mTLS provisioning . **ThingsBoard** leads as the most popular open-source IoT platform . **Kaa IoT** delivers enterprise IoT with a Kubernetes-ready, microservices architecture . This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[AWS IoT Core](https://aws.amazon.com/iot-core/)**  

  **AWS's managed IoT connectivity service** — connect billions of IoT devices and route trillions of messages to AWS services . **Supports MQTT, HTTPS, MQTT over WSS, and LoRaWAN** . **Mutual authentication with X.509 certificates** and fine-grained access control via IAM policies . **Device Shadow for offline state management** and **Rules Engine for message routing** . **Best for AWS-native IoT connectivity** .



- **[Azure IoT Hub](https://azure.microsoft.com/en-us/products/iot-hub/)**  

  **Microsoft's managed IoT connectivity platform** — bidirectional communication between IoT devices and Azure . **Supports MQTT, AMQP, and HTTPS with per-device authentication** . **Device-to-cloud and cloud-to-device messaging with built-in routing** . **Best for Azure-native IoT connectivity** .



- **[Google Cloud IoT](https://cloud.google.com/solutions/iot)**  

  **Google's IoT connectivity** — Pub/Sub for device messaging with Cloud IoT Core (now retired) . **Recommended alternatives include Pub/Sub, Dataflow, and partner MQTT brokers** . **Best for GCP-native IoT architectures** .



- **[Particle](https://www.particle.io/)**  

  **IoT platform for connected devices** — cellular and Wi-Fi modules with cloud connectivity, OTA updates, and device management . **Best for prototyping and production IoT** .



- **[EMQX Cloud](https://www.emqx.com/)**  

  **Managed MQTT broker** — scalable to 100M+ connections . **Best for large-scale IoT messaging** . **Open-source EMQX also available for self-hosting** .



- **[HiveMQ Cloud](https://www.hivemq.com/)**  

  **Managed MQTT broker** — enterprise-grade IoT messaging . **Free tier available**; paid plans for production . **Best for IoT messaging** . **Open-source HiveMQ Community Edition also available** .



- **[Losant](https://www.losant.com/)**  

  **Enterprise IoT application platform** — visual workflow builder, edge compute, and device management . **Best for enterprise IoT** .



- **[ThingsBoard](https://thingsboard.io/)**  

  **Open-source IoT platform** — see Open-Source section for the community edition.



- **[Ayla Networks](https://www.aylanetworks.com/)**  

  **IoT platform for connected products** — device connectivity, data management, and application enablement . **Best for consumer and commercial IoT** .



- **[Kaa IoT](https://www.kaaiot.com/)**  

  **Enterprise IoT platform** — see Open-Source section for the community edition.



## Open-Source GitHub Projects



### MQTT Brokers



- **[EMQX](https://github.com/emqx/emqx)**  

  **The most scalable open-source MQTT broker**, Apache-2.0 licensed with **13,000+ GitHub stars** . **Connects 100M+ IoT devices and processes 1M+ messages per second** . **Built for high reliability and low latency** . **Supports MQTT 5.0, MQTT-SN, CoAP, LwM2M, and more** . **Cluster-ready with auto-discovery** . **Built-in rule engine for message processing** . **Best for large-scale IoT messaging** .



- **[Eclipse Mosquitto](https://github.com/eclipse/mosquitto)**  

  **The reference lightweight MQTT broker**, EPL-2.0 licensed with **8,000+ GitHub stars** . **Implements MQTT 5.0, 3.1.1, and 3.1** . **Low resource consumption** — runs on embedded devices and single-board computers . **Bridge support for connecting to remote brokers** . **Best for simple, resource-constrained IoT messaging** .



- **[NanoMQ](https://github.com/nanomq/nanomq)**  

  **Ultra-lightweight MQTT broker for edge**, MIT licensed . **Only 1.7MB in size** — designed for resource-constrained edge gateways . **Built on NNG with multi-threaded architecture** . **Supports MQTT 5.0/3.1.1, bridging, and rule engine** . **Best for edge MQTT deployments** .



- **[VerneMQ](https://github.com/vernemq/vernemq)**  

  **Distributed MQTT broker**, Apache-2.0 licensed . **Clusters to 100+ nodes with auto-discovery** . **Scales to millions of concurrent connections** . **Supports MQTT 5.0, WebSocket, and bridge mode** . **Best for clustered MQTT deployments** .



- **[HiveMQ Community Edition](https://github.com/hivemq/hivemq-community-edition)**  

  **Open-source MQTT broker with enterprise-grade semantics**, Apache-2.0 licensed . **Backpressure handling and high throughput** . **Supports MQTT 5.0 and 3.x** . **Best for IoT messaging with enterprise semantics** .



- **[Moquette](https://github.com/moquette-io/moquette)**  

  **Java MQTT broker**, Apache-2.0 licensed . **Lightweight and embeddable** . **Supports MQTT 3.1 and 3.1.1** . **Best for Java-based IoT messaging** .



### IoT Connectivity Platforms



- **[Magistrala](https://github.com/absmach/magistrala)**  

  **Modern, Go-based, cloud-native IoT platform framework** (formerly Mainflux), Apache-2.0 licensed . **Supports MQTT, CoAP, HTTP, WebSocket, and LoRaWAN** . **Provision utility** creates channels and clients with certificate generation for mTLS use cases . **Fine-grained access control** — define object-scoped roles like "reader on channel1" . **Atom integration model** provides identity, authorization, and catalog with workspaces, entities, resources, and groups . **Scales from simple prototypes to complex deployments** without rigid patterns . **Best for cloud-native IoT connectivity with security** .



- **[ThingsBoard](https://github.com/thingsboard/thingsboard)**  

  **The most popular open-source IoT platform with 17,000+ GitHub stars**, Apache-2.0 licensed . **Supports MQTT, CoAP, HTTP, LwM2M, SNMP** . **Device management, data collection, processing, and visualization** . **Rule Engine for event-based workflows** . **Multi-tenancy with RBAC** . **Security**: Two-Factor Authentication, OAuth 2.0, Access Tokens, X.509 Certificates, SSL, DTLS . **Trade-offs**: Can be resource-heavy; Community edition lacks many Professional features . **Best for comprehensive IoT platform** .



- **[Kaa IoT Platform](https://github.com/kaaproject/kaa)**  

  **Enterprise IoT platform with open-source core**, Apache-2.0 licensed . **Kubernetes-ready, microservices architecture** — modular and extensible . **Device management, data collection, and OTA updates** . **SDKs for C, C++, Java, Python, and more** . **Best for enterprise IoT with Kubernetes** .



- **[Mainflux (archived)](https://github.com/mainflux/mainflux)** — Original Mainflux project, now continued as Magistrala .



- **[OpenHAB](https://github.com/openhab/openhab-core)** — Vendor-neutral home automation with MQTT binding .



- **[Home Assistant](https://github.com/home-assistant/core)** — Open-source home automation with extensive IoT integrations .



### Edge Connectivity



- **[Mongoose OS](https://github.com/cesanta/mongoose-os)** — IoT firmware with MQTT, OTA, and cloud integrations .



- **[EdgeX Foundry](https://github.com/edgexfoundry/edgex-go)** — Vendor-neutral IoT edge platform with MQTT and device connectivity .



- **[EMQX Edge](https://github.com/emqx/emqx)** — Lightweight edge MQTT broker from EMQX .



### Additional Strong Open-Source Options



- **MQTT.js** — MQTT client library for JavaScript .

- **Paho MQTT** — Eclipse Paho MQTT client libraries for C, C++, Python, Java, Go, and more .

- **Paho Embedded C** — MQTT client for embedded systems .

- **tinyMQTT** — Minimal MQTT broker in Python .

- **Aedes** — Barebone MQTT server for Node.js .

- **Mosca** — MQTT broker for Node.js (predecessor to Aedes) .

- **RabbitMQ MQTT Adapter** — MQTT support for RabbitMQ .

- **NATS** — Cloud-native messaging with MQTT support via NATS MQTT .

- **Apache Kafka** — Event streaming with MQTT Connect via Kafka Connect .



**Frameworks for building custom IoT cloud connectivity and messaging solutions**: Combine **EMQX** for large-scale IoT messaging with 100M+ connection support . Use **Mosquitto** or **NanoMQ** for resource-constrained edge deployments . Deploy **VerneMQ** for clustered MQTT with 100+ nodes . Choose **HiveMQ Community Edition** for enterprise-grade MQTT semantics . Integrate **Magistrala** for cloud-native IoT connectivity with fine-grained access control and mTLS . Use **ThingsBoard** or **Kaa IoT** for comprehensive IoT platforms with rule engines and dashboards . Note that true managed IoT connectivity with global infrastructure, automatic scaling, and vendor-supported SLAs (AWS IoT Core, Azure IoT Hub, EMQX Cloud) remains primarily commercial territory; open-source stacks provide strong MQTT brokers, device connectivity, and IoT platform foundations that require integration for complete IoT cloud messaging.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- IoT connectivity platforms handle device credentials and control physical devices. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.

- **MQTT broker choice depends on scale** — Mosquitto for lightweight, EMQX for 100M+ connections, NanoMQ for edge, VerneMQ for clustering . Benchmark against your specific workload.

- **Security is critical** — use TLS/SSL, client certificates, and authentication. Never expose MQTT brokers directly to the internet without proper security controls .

- **Google Cloud IoT Core was retired** in 2023 — migrate to Pub/Sub with partner MQTT brokers for new deployments .

- **License considerations**: EMQX uses Apache-2.0, Mosquitto uses EPL-2.0, NanoMQ uses MIT, VerneMQ uses Apache-2.0, HiveMQ Community uses Apache-2.0, and Magistrala uses Apache-2.0. Verify licensing against your use case before committing.

- The open-source ecosystem provides strong MQTT brokers, device connectivity, and IoT platform foundations, but **managed infrastructure, global scale, and vendor-supported SLAs** remain primarily commercial offerings.



---



**Made for IoT engineers, embedded developers, and organizations seeking IoT cloud connectivity sovereignty.**  

Let's make IoT cloud connectivity and messaging more open, transparent, and scalable.
