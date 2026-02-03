# Google Summer of Code 2026

## [![Google Summer of Code 2026](https://github.com/Sing-Li/bbug/raw/master/images/gsoclogo.jpg)](https://summerofcode.withgoogle.com)

## How to apply

Gojek has applied as a mentoring open source organization for Google Summer of Code 2026.  See [official Google Summer of Code site](https://summerofcode.withgoogle.com/).

Gojek is proud to apply for Google Summer of Code for the first time, joining the global effort to nurture the next generation of open source contributors.  

We welcome aspiring developers from around the world, https://opensource.googleblog.com/2021/11/expanding-google-summer-of-code-in-2022.html, who are passionate about coding and  eager to explore the world of open source to join us as GSoC 2026 contributors.  

For details and rules of Google Summer of Code 2026, please see the [GSoC 2026 Official Website](https://summerofcode.withgoogle.com/). 

For timeline, see [Official Google Summer of Code 2026 Timeline](https://developers.google.com/open-source/gsoc/timeline) for more details.

We encourage authentic, original work. While AI tools may be used for research or translation, proposals generated entirely by LLMs or AI agents will be rejected. You must write your proposal yourself and be able to justify every detail if invited for an interview. A demonstrable track record of GitHub contributions will also improve your chances of selection for GSoC 2026. See [Google's Contributors Guide on using AI tooling in GSoC 2026](https://docs.google.com/document/d/1t9GcIBnNXPNO6klRQvU8pL8-uV6afzLo6JUAM299suA/edit?tab=t.0#heading=h.tgbr0z4x9eg5) for some suggestions.

### **Contacting Gojek Team**

Interested contributors are encouraged to interact directly with our team and community  on our community channel for Google Summer of Code 2026 : [https://discord.com/channels/google-summer-of-code-2026](https://discord.com/channels/986889666651373568/1468219617066356807)

As well as on GitHub: [https://github.com/gojek/](https://github.com/gojek/)

---


## 📂 Project Ideas   

### **Total Projects : 8**


### 1. TraceDump: Tcpdump-like Tracing Tool for MQTT Traffic

👥 **Mentor(s):** Dhruv Jain, Vivek Pipaliya

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
    The existing vmq-admin tracing functionality in Gojek's VerneMQ fork is limited to a single session and lacks filtering by topics, users, or MQTT packet types. This project aims to build a tcpdump-like tracing tool for VerneMQ that supports multiple concurrent tracing sessions, fine-grained filtering, and real-time dumping of MQTT events to external files.

💪 **Desired Skills:** Erlang, MQTT, Redis

🎯 **Goals/Deliverables:**
  - Support for concurrent tracing of multiple clients or sessions on a single node
  - Fine-grained filtering by topic, username, client ID, and MQTT packet type
  - Real-time dumping of MQTT events to external files
  - Optional replay or playback of captured traces for analysis and debugging

⏳ **Project Duration:** 90 hours

📈 **Difficulty:** Intermediate

-----

### 2. gRPC-Based Webhook Events Plugin for MQTT Broker

👥 **Mentor(s):** Dhruv Jain, Vivek Pipaliya

📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
Gojek's VerneMQ fork currently provides webhook event streaming through the vmq_events_sidecar, which uses a plain TCP connection to deliver events asynchronously. While functional, this approach requires operators to implement and maintain a custom TCP server, lacks strong interface contracts, and offers limited flexibility for structured, bidirectional communication. The present webhook events plugin is using HTTP/1.1 that affects the broker's performance at high load.
The goal of this project is to design and implement a new VerneMQ webhook events plugin based on gRPC, enabling structured, strongly-typed event delivery with support for both asynchronous streaming and synchronous request–response modes.

💪 **Desired Skills:** Erlang, MQTT, GRPC, Redis

🎯 **Goals/Deliverables:**
  - Implement a gRPC-based webhook events plugin
  - Support both asynchronous event streaming and synchronous event handling
  - Provide clearly defined protobuf schemas for webhook events
  - Enable configurable delivery modes, timeouts, and retry semantics
  - Ensure minimal performance impact and safe backpressure handling
  - Load test using MzBench for 10,000 rps send/receive rate with 100K concurrent connections

⏳ **Project Duration:** 175 hours

📈 **Difficulty:** Intermediate

-----

### 3. MQTT over QUIC Support in Broker
👥 **Mentor(s):** Anubhav Gupta, Dhruv Jain
📢 **Communication Channel:** [Gojek Courier Discord Channel](https://discord.com/channels/986889666651373568/1468219617066356807)

📝 **Repository:** https://github.com/gojek/vernemq

💬 **Description:**
This project aims to add support for MQTT connections over the QUIC protocol as an additional listener option in VerneMQ. It must allow MQTT clients to connect using QUIC while preserving MQTT protocol semantics and security guarantees.

💪 **Desired Skills:** Erlang, MQTT, QUIC, Redis

🎯 **Goals/Deliverables:**
  - Add a QUIC listener option to VerneMQ alongside existing TCP/TLS listeners
  - Support secure connections using TLS 1.3 as required by QUIC
  - Ensure compatibility with existing MQTT protocol versions and client libraries
  - Handle session lifecycle, flow control, and backpressure appropriately
  - Stress test to evaluate performance, latency, and resource usage compared to TCP/TLS
  - Document configuration, limitations, and best practices

⏳ **Project Duration:** 175 hours

📈 **Difficulty:** Intermediate
