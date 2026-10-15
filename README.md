# Aashutosh Bairagi

### Full-Stack Developer · Real-Time Systems · AI Agents

I build full-stack products with a focus on **real-time communication, AI agent systems, and backend engineering**.

Currently building **[WebChat](https://webchat.qzz.io)** and **[ARC-AI](https://arc-ai-project.vercel.app/)** — two projects that push me to work beyond the happy path: streaming, synchronization, memory, failure recovery, and the engineering decisions that make applications feel reliable.

[Portfolio](https://aashutoshbairagi.vercel.app/) · [GitHub](https://github.com/Aashutosh31) · [LinkedIn](https://www.linkedin.com/in/aashutosh-bairagi-559aa530b/) · [X](https://x.com/Aashutosh_dev31)

---

## About

I'm a computer science student and independent developer who enjoys understanding how software works beneath the interface.

My interests sit at the intersection of:

- **Real-time engineering** — event delivery, WebSockets, WebRTC, and synchronized state.
- **AI systems** — streaming inference, tool orchestration, retrieval-augmented generation, and conversational memory.
- **Backend engineering** — APIs, authentication, caching, persistence, and failure handling.
- **Infrastructure** — Docker, deployment workflows, and maintainable system architecture.

I learn by building real products, debugging the difficult parts, and improving the underlying design.

```text
~/engineering
├── webchat/     # Real-time social communication
├── arc-ai/      # Conversational AI and agent runtime
└── experiments/ # Learning through implementation
```

## Featured Projects

### 01. WebChat

**A real-time social communication platform**

[Open WebChat ↗](https://webchat.qzz.io) · [System Design & Documentation ↗](https://github.com/Aashutosh31/webchat-system-design)

WebChat brings persistent messaging, communities, discussion spaces, and ephemeral social content together in one product.

**Engineering highlights**

- **Distributed event delivery:** Redis Pub/Sub helps synchronize real-time events across multiple Socket.IO server instances.
- **Voice and video:** LiveKit provides infrastructure for multi-party WebRTC communication.
- **Authentication:** JWT-based access and refresh-token flows support session management.
- **Cryptography:** Browser-native Web Crypto APIs support encryption for selected payloads.
- **Containerization:** Docker helps separate application services and supporting infrastructure.
- **Integrated AI:** An embedded assistant brings contextual AI capabilities into the communication experience.

**Stack**

`React` `TypeScript` `Node.js` `MongoDB` `Redis` `Socket.IO` `LiveKit` `Docker` `Tailwind CSS`

---

### 02. ARC-AI

**A real-time conversational assistant and AI agent runtime**

[Try the live demo ↗](https://arc-ai-project.vercel.app/) · [Explore the source code ↗](https://github.com/Aashutosh31/arc-ai-project)

ARC-AI is an AI workspace built around streaming responses, tool execution, conversational voice, vision, and retrieval-based memory.

**Engineering highlights**

- **Incremental streaming:** Responses arrive progressively instead of waiting for the entire completion.
- **Multi-step tool execution:** The agent can invoke tools, process their results, and continue its execution.
- **Retrieval-based memory:** Relevant historical context can be retrieved instead of repeatedly supplying the entire conversation history.
- **Interruptible voice:** A voice interaction state machine handles conversational turn-taking and user interruptions.
- **Provider resilience:** Recovery logic helps manage failed model calls without unnecessarily breaking execution continuity.
- **Runtime optimization:** Improvements to delivery and persistence paths reduce avoidable delays in the streaming experience.

**Stack**

`React` `Node.js` `MongoDB` `Socket.IO` `LLM APIs` `RAG` `Vector Search` `STT/TTS`

---

## Engineering Interests

| Domain | Areas of focus |
| --- | --- |
| AI agents | Tool calling, orchestration, RAG, semantic memory |
| Real-time systems | WebSockets, WebRTC, event propagation, synchronization |
| Backend | Node.js, API design, authentication, caching |
| Data | MongoDB, Redis, vector retrieval |
| Infrastructure | Docker, deployment, service boundaries |
| Developer tooling | Git, Linux, automation, technical documentation |

## Tech Stack

**Frontend**

React · JavaScript · TypeScript · Tailwind CSS · Zustand · Framer Motion

**Backend**

Node.js · Express · Socket.IO · REST APIs

**Data and AI**

MongoDB · Redis · Pinecone · LLM APIs · Retrieval-Augmented Generation

**Real-Time Infrastructure**

WebSockets · WebRTC · LiveKit · Streaming pipelines · Speech interfaces

**DevOps and Tools**

Docker · Git · GitHub · Vercel · Render

**Development Environment**

Arch Linux · Hyprland · Omarchy · VS Code · JetBrains Mono

## Currently Working On

- Improving WebChat's real-time communication and community experience.
- Refining ARC-AI's voice interaction, tool execution, and runtime reliability.
- Strengthening my understanding of distributed systems and backend architecture.
- Building better development workflows and documenting technical decisions.

## Beyond the Code

I use Arch Linux with Hyprland and enjoy building a keyboard-driven development environment.

I like the parts of engineering that require digging deeper: tracing a race condition, understanding a latency bottleneck, or figuring out why a system behaves differently under failure.

**My goal is to build software that is not only functional, but thoughtfully engineered.**

## Connect

- **Portfolio:** https://aashutoshbairagi.vercel.app/
- **GitHub:** https://github.com/Aashutosh31
- **LinkedIn:** https://www.linkedin.com/in/aashutosh-bairagi-559aa530b/
- **X:** https://x.com/Aashutosh_dev31

---

*Build. Debug. Understand. Improve.*
