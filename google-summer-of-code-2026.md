# Google Summer of Code 2026

## [![Google Summer of Code 2026](https://github.com/Sing-Li/bbug/raw/master/images/gsoclogo.jpg)](https://summerofcode.withgoogle.com)

We welcome aspiring developers from around the world, https://opensource.googleblog.com/2021/11/expanding-google-summer-of-code-in-2022.html, who are passionate about coding and  eager to explore the world of open source to join us as GSoC 2026 contributors.

For details and rules of Google Summer of Code 2026, please see the [GSoC 2026 Official Website](https://summerofcode.withgoogle.com/). 

For timeline, refer the [Official Google Summer of Code 2026 Timeline](https://developers.google.com/open-source/gsoc/timeline).

We encourage authentic, original work. While AI tools may be used for research or translation, proposals generated entirely by LLMs or AI agents will be rejected. You must write your proposal yourself and be able to justify every detail if invited for an interview. A demonstrable track record of GitHub contributions will also improve your chances of selection for GSoC 2026. See [Google's Contributors Guide on using AI tooling in GSoC 2026](https://docs.google.com/document/d/1t9GcIBnNXPNO6klRQvU8pL8-uV6afzLo6JUAM299suA/edit?tab=t.0#heading=h.tgbr0z4x9eg5) for some suggestions.

### **Contacting Gojek Team**

Interested contributors are encouraged to interact directly with our team and community  on our 24 x 7 community channel for Google Summer of Code 2026 : [https://discord.com/channels/google-summer-of-code-2026](https://discord.com/channels/986889666651373568/1468219617066356807)

As well as on GitHub: [https://github.com/gojek/](https://github.com/gojek/)

---


## 📂 Project Ideas   

### **Total Project Ideas : 14**
(Please note that this is an evolving list of project ideas. Feel free to propose and discuss new ideas as we continue to add more)

### 1. MQTT over QUIC in Courier Android Library

👥 **Mentor(s):** Deepanshu, Anubhav Gupta

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/courier-android

💬 **Description:**
Traditionally, MQTT runs over TCP/TLS, which can suffer from higher connection latency, head-of-line blocking, and suboptimal performance in mobile and unreliable network environments. This project proposes adding MQTT over QUIC support to the Courier library. QUIC is a modern transport protocol built on UDP that provides faster connection establishment, improved multiplexing, better congestion control, and seamless connection migration. By supporting MQTT over QUIC, Courier can offer lower latency, improved reliability on mobile networks, and better overall performance compared to traditional TCP-based transports.

💪 **Desired Skills:** Kotlin, MQTT, QUIC

🎯 **Goals/Deliverables:**
  - Design and implementation of a QUIC-based transport layer for Courier
  - Abstraction of the transport layer to support multiple protocols (TCP, QUIC)
  - Integration of MQTT protocol handling over QUIC streams
  - Configuration options for enabling and tuning QUIC transport
  - Performance benchmarking and comparison with TCP/TLS

⏳ **Project Duration:** Medium (~175 hours)

📈 **Difficulty:** Intermediate

-----

### 2. MQTTv5: MQTT version 5 support in Courier Android Library

👥 **Mentor(s):** Deepanshu, Anubhav Gupta

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/courier-android

💬 **Description:**
This project aims to add first-class MQTTv5 support to the Courier library while preserving backward compatibility with existing MQTT versions. MQTTv5 introduces significant enhancements such as reason codes, user properties, session and flow control improvements, request–response patterns, and better error handling. Supporting MQTTv5 will allow Courier users to build more robust, observable, and feature-rich messaging systems.

💪 **Desired Skills:** Kotlin, MQTT

🎯 **Goals/Deliverables:**
  - Full or substantial support for MQTT version 5 features in Courier
  - Backward compatibility with existing MQTTv3.x integrations
  - API extensions to expose MQTTv5 capabilities cleanly
  - Unit and integration tests covering MQTTv5 scenarios

⏳ **Project Duration:** Medium (~175 hours)

📈 **Difficulty:** Intermediate

-----

### 3. Courier Multiplatform: Kotlin Multi Platform compatible Courier Library

👥 **Mentor(s):** Deepanshu, Anubhav Gupta

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/courier-android

💬 **Description:**
This project aims to evolve Courier into a Kotlin Multiplatform (KMP) compatible library, allowing a single shared codebase to be used consistently across Android, iOS, and backend services. The work will involve refactoring core modules, introducing multiplatform abstractions, modularizing platform-specific logic, and ensuring backward compatibility with existing Android and JVM integrations.

💪 **Desired Skills:** Kotlin, MQTT, Android

🎯 **Goals/Deliverables:**
  - Courier core refactored to support Kotlin Multiplatform
  - Clear separation between common and platform-specific modules
  - Stable and backward-compatible APIs for existing users
  - Usable Courier integrations on Android, JVM/backend, and iOS
  - Improved documentation and examples for multiplatform usage

⏳ **Project Duration:** Medium (~175 hours)

📈 **Difficulty:** Intermediate

-----

### 4. Courier Proxy: Mqtt Event Visualising & Debugging application

👥 **Mentor(s):** Deepanshu, Anubhav Gupta

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/courier-android

💬 **Description:**
This project proposes building Courier Proxy, an intermediate MQTT proxy and visualization tool that sits between MQTT clients and brokers. The proxy will intercept, inspect, and optionally persist MQTT events, providing developers with real-time visibility into message flows. The tool will help visualize connections, subscriptions, publishes, acknowledgements, and errors, significantly improving debugging, performance analysis, and operational observability for Courier-based systems

💪 **Desired Skills:** Kotlin/Swift, Android/iOS, MQTT

🎯 **Goals/Deliverables:**
  - A functional MQTT proxy capable of intercepting and forwarding traffic
  - Real-time visualization of MQTT events and message flows
  - Improved developer experience for debugging Courier and MQTT-based systems
  - A reusable debugging and observability tool for local and staging environments

⏳ **Project Duration:** Medium (~175 hours)

📈 **Difficulty:** Intermediate

-----

### 5. Connection Pooling support in Courier Library

👥 **Mentor(s):** Deepanshu, Anubhav Gupta

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/courier-android

💬 **Description:**
This project aims to introduce connection pooling support into the Courier library. The pooling mechanism will allow multiple logical Courier clients to efficiently share a managed set of underlying MQTT connections, improving performance, reducing connection churn, and optimizing system resource usage. The solution will be designed to be configurable, backward-compatible, and safe for concurrent usage.

💪 **Desired Skills:** Kotlin, MQTT

🎯 **Goals/Deliverables:**
  - Design and implementation of a connection pooling abstraction in Courier
  - A clean, extensible connection pooling API within Courier
  - Thread-safe and concurrency-safe pool management
  - Graceful connection lifecycle handling (creation, reuse, eviction, shutdown)

⏳ **Project Duration:** Small (~90 hours)

📈 **Difficulty:** Intermediate

-----

### 6. MQTT for Fleet Telematics in Courier Android

👥 **Mentor(s):** Deepanshu, Anubhav Gupta

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/courier-android

💬 **Description:**
This project aims to design and implement a robust MQTT-based communication framework for fleet telematics using the Courier library. The focus will be on reliable ingestion, transport, and processing of telemetry data such as GPS coordinates, vehicle health metrics, sensor readings, and event signals. The project will explore MQTT features such as Quality of Service (QoS), session persistence, offline buffering, and efficient topic design to meet the unique requirements of fleet-scale telematics systems.

💪 **Desired Skills:** Android, Kotlin, MQTT

🎯 **Goals/Deliverables:**
  - Design of an MQTT-based telematics communication model
  - Courier-based client implementation for vehicle or edge devices
  - Improved handling of intermittent connectivity and mobile networks
  - Reusable patterns and best practices for large-scale IoT and fleet systems

⏳ **Project Duration:** Small (~90 hours)

📈 **Difficulty:** Intermediate

-----

### 7. OpenTelemetry Support in Golang Paho Library

👥 **Mentor(s):** Ken Kalang Al Qalyubi, Paras Sharma

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/paho.mqtt.golang

💬 **Description:**
  The Golang Paho MQTT client library provides basic metrics and logging capabilities but lacks native integration with modern observability standards such as OpenTelemetry (OTel). The goal of this project is to add OpenTelemetry-based instrumentation to the Golang Paho MQTT library, enabling applications to export Prometheus-compatible metrics and integrate seamlessly with existing observability pipelines.

💪 **Desired Skills:** MQTT, Golang, Paho, OpenTelemetry, Prometheus

🎯 **Goals/Deliverables:**
  - Add OpenTelemetry metrics instrumentation to the Golang Paho MQTT library
  - Expose key MQTT client metrics such as connection state, publish/subscribe rates, latency, and error counts
  - Support Prometheus-compatible metric export via OpenTelemetry
  - Ensure instrumentation is optional and configurable with minimal runtime overhead
  - Preserve backward compatibility and existing public APIs
  - Provide documentation and examples for integrating OTel and Prometheus

⏳ **Project Duration:** Medium (~175 hours)

📈 **Difficulty:** Intermediate

-----

### 8. MQTT v5 Support in the courier-go Library

👥 **Mentor(s):** Paras Sharma, Ken Kalang Al Qalyubi

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/courier-go

💬 **Description:**
The goal of this project is to add first-class MQTT v5 support to the courier-go library ensuring correctness, stability, and compatibility of MQTT v5 operations.

💪 **Desired Skills:** MQTT, Golang, Paho

🎯 **Goals/Deliverables:**
  - Implement full MQTT v5 protocol support in courier-go
  - Support MQTT v5 properties, reason codes, and enhanced acknowledgements
  - Enable user-configurable session expiry, message expiry, and flow control
  - Maintain compatibility with existing MQTT v3.x users of the library
  - Add comprehensive tests and examples covering MQTT v5 behavior
  - Document API changes, migration paths, and best practices

⏳ **Project Duration:** Medium (~175 hours)

📈 **Difficulty:** Intermediate

-----

### 9. ClientID-Based Rate Limiting for MQTT Events in Broker

👥 **Mentor(s):** Vivek Pipaliya, TBD

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
VerneMQ currently does not provide a built-in mechanism to rate-limit MQTT operations on a per-client basis. As a result, a single misbehaving or malicious client can overwhelm the broker with excessive CONNECT, PUBLISH, or SUBSCRIBE requests, potentially degrading performance or impacting other connected clients.

The goal of this project is to design and implement a ClientID-based rate limiter within VerneMQ to control the rate of MQTT events and improve the broker’s security and stability.

💪 **Desired Skills:** MQTT, Erlang, VerneMQ, Redis, MzBench

🎯 **Goals/Deliverables:**
  - Implement configurable, per-ClientID rate limits for MQTT operations
  - Support different limits for CONNECT, PUBLISH, SUBSCRIBE, and UNSUBSCRIBE
  - Define clear enforcement actions (throttle, delay, disconnect, or reject)
  - Ensure minimal performance overhead and safe concurrency handling
  - Integrate cleanly with existing authentication and hook mechanisms
  - Provide observability via metrics and logs

⏳ **Project Duration:** Small (~90 hours)

📈 **Difficulty:** Intermediate

-----

### 10. Stable MQTT v5 Support in Broker & MZBench

👥 **Mentor(s):** Vivek Pipaliya, TBD

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
This project aims to add stable and production-ready MQTT v5 support to Gojek's VerneMQ fork and load-testing tool MZBench using vmq_mzbench plugin.

On the broker side, the goal is to ensure correctness, stability, and compatibility of MQTT v5 behavior across core broker operations and extension points.

In parallel, MQTT v5 support needs to be added to MZBench, enabling comprehensive load and stress testing of MQTT v5 features.

💪 **Desired Skills:** MQTT v5 and v3.1.1, Erlang, VerneMQ, Redis, MzBench

🎯 **Goals/Deliverables:**
  - Implement and stabilize MQTT v5 support in Gojek's VerneMQ fork (connect, publish, subscribe, unsubscribe, disconnect)
  - Ensure correct handling of MQTT v5 properties and reason codes by adding unit & end to end common tests
  - Validate compatibility with Redis-backed state and hook-based extensions
  - Extend MZBench to support MQTT v5 clients and workloads
  - Enable end-to-end load testing and benchmarking of MQTT v5 features
  - Identify and document performance characteristics and limitations

⏳ **Project Duration:** Large (~350 hours)

📈 **Difficulty:** Hard

-----

### 11. Direct Kafka Integration as an MQTT Subscriber on Broker 

👥 **Mentor(s):** Dhruv Jain, Vivek Pipaliya

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
This project aims to add native Kafka integration to Gojek's VerneMQ fork by implementing a built-in MQTT subscriber that forwards messages published on designated MQTT topics directly to Kafka.

The integration will allow operators to configure special or mapped MQTT topics that are consumed internally by the broker and published to corresponding Kafka topics, enabling seamless data pipelines from MQTT producers to Kafka consumers without requiring external bridge services.

💪 **Desired Skills:** MQTT, Kafka, Erlang, VerneMQ, Redis, MzBench

🎯 **Goals/Deliverables:**
  - Implement a native MQTT subscriber within Gojek's VerneMQ fork for Kafka integration
  - Support configurable mapping between MQTT topics and Kafka topics
  - Preserve MQTT QoS semantics when publishing messages to Kafka
  - Support message keying, partitioning strategies, and headers where applicable
  - Provide backpressure handling and failure recovery to avoid broker overload
  - Stress & chaos test using MzBench to document broker's kafka message throughput handling capacity

⏳ **Project Duration:** Large (~350 hours)

📈 **Difficulty:** Hard

-----

### 12. TraceDump: Tcpdump-like Tracing Tool for MQTT Traffic

👥 **Mentor(s):** Dhruv Jain, Vivek Pipaliya

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
    The existing vmq-admin tracing functionality in Gojek's VerneMQ fork is limited to a single session and lacks filtering by topics, users, or MQTT packet types. This project aims to build a tcpdump-like tracing tool for VerneMQ that supports multiple concurrent tracing sessions, fine-grained filtering, and real-time dumping of MQTT events to external files.

💪 **Desired Skills:** Erlang, MQTT, Redis, VerneMQ

🎯 **Goals/Deliverables:**
  - Support for concurrent tracing of multiple clients or sessions on a single node
  - Fine-grained filtering by topic, username, client ID, and MQTT packet type
  - Real-time dumping of MQTT events to external files
  - Optional replay or playback of captured traces for analysis and debugging

⏳ **Project Duration:** Small (~90 hours)

📈 **Difficulty:** Intermediate

-----

### 13. gRPC-Based Webhook Events Plugin for MQTT Broker

👥 **Mentor(s):** Dhruv Jain, Vivek Pipaliya

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
Gojek's VerneMQ fork currently provides webhook event streaming through the vmq_events_sidecar, which uses a plain TCP connection to deliver events asynchronously. While functional, this approach requires operators to implement and maintain a custom TCP server, lacks strong interface contracts, and offers limited flexibility for structured, bidirectional communication. The present webhook events plugin is using HTTP/1.1 that affects the broker's performance at high load.
The goal of this project is to design and implement a new VerneMQ webhook events plugin based on gRPC, enabling structured, strongly-typed event delivery with support for both asynchronous streaming and synchronous request–response modes.

💪 **Desired Skills:** Erlang, MQTT, GRPC, Redis, VerneMQ

🎯 **Goals/Deliverables:**
  - Implement a gRPC-based webhook events plugin
  - Support both asynchronous event streaming and synchronous event handling
  - Provide clearly defined protobuf schemas for webhook events
  - Enable configurable delivery modes, timeouts, and retry semantics
  - Ensure minimal performance impact and safe backpressure handling
  - Load test using MzBench for 10,000 rps send/receive rate with 100K concurrent connections

⏳ **Project Duration:** Medium (~175 hours)

📈 **Difficulty:** Intermediate

-----

### 14. MQTT over QUIC Support in Broker

👥 **Mentor(s):** Anubhav Gupta, Dhruv Jain

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
This project aims to add support for MQTT connections over the QUIC protocol as an additional listener option in VerneMQ. It must allow MQTT clients to connect using QUIC while preserving MQTT protocol semantics and security guarantees.

💪 **Desired Skills:** Erlang, MQTT, QUIC, Redis, VerneMQ

🎯 **Goals/Deliverables:**
  - Add a QUIC listener option to VerneMQ alongside existing TCP/TLS listeners
  - Support secure connections using TLS 1.3 as required by QUIC
  - Ensure compatibility with existing MQTT protocol versions and client libraries
  - Handle session lifecycle, flow control, and backpressure appropriately
  - Stress test to evaluate performance, latency, and resource usage compared to TCP/TLS
  - Document configuration, limitations, and best practices

⏳ **Project Duration:** Medium (~175 hours)

📈 **Difficulty:** Intermediate
