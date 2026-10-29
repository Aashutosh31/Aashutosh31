<div align="center">
  <img src="assets/hero.svg" alt="Aashutosh Bairagi — Full-Stack Engineer, Real-Time Systems, AI Agents" width="100%" />
</div>

<div align="center">

<a href="https://aashutoshbairagi.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-1a1b26?style=flat-square&logo=vercel&logoColor=7dcfff" alt="Portfolio" /></a>
<a href="https://www.linkedin.com/in/aashutosh-bairagi-559aa530b/"><img src="https://img.shields.io/badge/LinkedIn-1a1b26?style=flat-square&logo=linkedin&logoColor=7aa2f7" alt="LinkedIn" /></a>
<a href="https://x.com/Aashutosh_dev31"><img src="https://img.shields.io/badge/X-1a1b26?style=flat-square&logo=x&logoColor=c0caf5" alt="X" /></a>
<a href="https://github.com/Aashutosh31"><img src="https://img.shields.io/badge/GitHub-1a1b26?style=flat-square&logo=github&logoColor=bb9af7" alt="GitHub" /></a>

[![XERJ Corpus Hub contributor](https://hub.xerj.org/contributors/Aashutosh31/badge.svg)](https://hub.xerj.org/contributors/Aashutosh31)

</div>

I'm a computer science student and independent developer. I build full-stack products and spend most of my time on the difficult parts — real-time synchronization, AI streaming and memory, and the engineering decisions that make a system stay reliable under load and failure.

- **What I build** — full-stack products, real-time applications, and AI systems.
- **How I think** — architecture, debugging, reliability, and the trade-offs behind each decision.
- **How I grow** — algorithms in C++, Python, and clearer technical communication for engineering interviews.

---

## Featured Projects

### WebChat — Real-time social communication platform

<a href="https://webchat.qzz.io"><img src="assets/webchat-banner.svg" alt="WebChat — real-time social communication platform" width="100%" /></a>

WebChat brings persistent messaging, multi-channel communities, voice and video, a social feed, and ephemeral stories into a single product — with an embedded AI assistant layered into the communication experience.

- **Distributed event delivery** — a Redis Pub/Sub adapter keeps Socket.IO events synchronized across multiple server instances, so presence and messages stay consistent as the app scales beyond one process.
- **Voice and video** — LiveKit provides the infrastructure for multi-party WebRTC rooms.
- **Auth** — JWT access and refresh-token flows handle session lifecycle.
- **Payload encryption** — browser-native Web Crypto APIs encrypt selected payloads on the client.
- **Containers** — Docker separates the application services from supporting infrastructure.
- **Native mobile** — the product also ships as an installable Android app via Capacitor.

**Stack:** `React` `TypeScript` `Node.js` `MongoDB` `Redis` `Socket.IO` `LiveKit` `Docker` `Tailwind CSS` `Capacitor`

**Links:** [Live app](https://webchat.qzz.io) · [System design & docs](https://github.com/Aashutosh31/webchat-system-design) · [Android APK](https://github.com/Aashutosh31/webchat-system-design/releases/download/v1.0.0/webchat.apk)

### ARC-AI — Streaming AI agent runtime

<a href="https://arc-ai-project.vercel.app/"><img src="assets/arc-ai-banner.svg" alt="ARC-AI — streaming AI agent runtime with tool execution and memory" width="100%" /></a>

ARC-AI is an AI workspace built around progressive streaming, multi-step tool execution, conversational voice, live vision, and retrieval-based memory — with a provider-agnostic model router.

- **Incremental streaming** — responses arrive token by token over Socket.IO instead of waiting for a full completion, with persistence handled off the critical path.
- **Multi-step tool execution** — the agent invokes tools, reads their results, and continues, through a provider-independent tool registry.
- **Retrieval-based memory** — relevant historical context is retrieved on demand rather than resending the entire conversation each turn.
- **Interruptible voice** — a half-duplex voice state machine handles turn-taking and user barge-in.
- **Provider resilience** — a capability-aware router (Groq for text/tools, Gemini for multimodal) excludes providers that cannot serve a request and falls back cleanly, including mid-stream.
- **Sandboxed execution** — LLM-triggered code runs inside an ECMAScript (QuickJS/WASM) sandbox.

**Stack:** `React` `Node.js` `MongoDB` `Socket.IO` `LLM APIs` `RAG` `Pinecone` `STT/TTS`

**Links:** [Live demo](https://arc-ai-project.vercel.app/) · [Source code](https://github.com/Aashutosh31/arc-ai-project)

---

## Other Projects

### Receipts — 90-day accountability

<a href="https://aashutosh31.github.io/receipts/"><img src="assets/receipts-banner.svg" alt="Receipts — a 90-day accountability mobile app" width="100%" /></a>

A native Flutter app that tracks consistency over a 90-day commitment, built around an honest, local-first record of daily progress.

- **Offline-first** — a local Drift (SQLite) database keeps the app usable without connectivity and syncs with the backend.
- **Supabase backend** — authentication, Postgres data, and row-level security policies define exactly who can read and write what.
- **Native polish** — local notifications, timezone-aware scheduling, and a Riverpod-managed state layer.

**Stack:** `Flutter` `Dart` `Supabase` `PostgreSQL` `Drift` `Riverpod`

**Links:** [Website](https://aashutosh31.github.io/receipts/) · [Source code](https://github.com/Aashutosh31/receipts-app) · [Download APK](https://github.com/Aashutosh31/receipts-app/releases/download/v1.0.0/receipts-v1.0.0.apk)

### AttendTrack — Role-based college attendance

<a href="https://smart-attendance-frontend-seven.vercel.app"><img src="assets/attendtrack-banner.svg" alt="AttendTrack — role-based attendance system with face recognition" width="100%" /></a>

An attendance platform for colleges with separate dashboards for admins, HODs, faculty, coordinators, and students.

- **Role-based access** — a shared auth layer and role gates drive distinct dashboards and workflows per user type.
- **Face-recognition check-in** — face descriptors are enrolled and matched server-side with `face-api.js` on TensorFlow.js (WASM).
- **Auth sync** — Supabase handles identity while the backend verifies tokens and enforces authorization.

**Stack:** `React` `Vite` `Tailwind CSS` `Node.js` `Express` `MongoDB` `Supabase` `TensorFlow.js`

**Links:** [Live app](https://smart-attendance-frontend-seven.vercel.app) · [Backend source](https://github.com/Aashutosh31/smart-attendance-backend) · [Frontend source](https://github.com/Aashutosh31/smart-attendance-frontend)

### SIH Intelligence — Hackathon problem analyzer

<a href="https://sih-intelligent-problem-analyzer.vercel.app"><img src="assets/sih-banner.svg" alt="SIH Intelligence — analyzes hackathon problem statements into execution plans" width="100%" /></a>

Paste a Smart India Hackathon problem statement and it returns a structured execution plan: engineering interpretation, a difficulty and risk scorecard, a recommended stack, team-fit scoring, and task allocation.

- **AI where it helps** — Gemini interprets the problem statement into structured data.
- **Deterministic where it matters** — scoring, team-fit, and task allocation are application-owned logic, not model guesswork, so results stay explainable.

**Stack:** `React` `Vite` `Tailwind CSS` `Node.js` `Express` `MongoDB` `Gemini API`

**Links:** [Live app](https://sih-intelligent-problem-analyzer.vercel.app) · [Source code](https://github.com/Aashutosh31/SIH-Intelligent-Problem-Analyzer)

> **Also exploring — Sahaay (SIH26093).** A voice-first, multilingual triage prototype for a public helpline: AI extracts evidence-backed signals, but a fixed-weight engine computes the Stress & Vulnerability Index and every routing decision stays human-in-the-loop. A hackathon prototype, kept private for now.

---

## How I Engineer

The details I care about are the ones that show up when something goes wrong:

- **Design for failure, not just the happy path.** Streaming continues while a failed model call is retried or rerouted; voice recovers when a provider drops out mid-stream.
- **Separate concerns behind interfaces.** A provider-agnostic LLM router, a tool registry, and Docker service boundaries mean one component can change without rewriting the others.
- **Keep the critical path fast.** Streaming responses don't wait on persistence; retrieval fetches only the relevant context instead of the full history.
- **Keep humans in the loop for high-stakes decisions.** In the SIH triage work, the model extracts signals but deterministic, auditable logic produces the score.
- **Make state consistent.** Pub/Sub fan-out across Socket.IO instances and role-scoped access rules keep a distributed system behaving like one.

## Tech Stack

**Languages** — TypeScript · JavaScript · C++ · Dart · Python · Rust (learning)

**Frontend** — React · Vite · Tailwind CSS · Zustand · React Router · Framer Motion

**Mobile** — Flutter · Capacitor · Android

**Backend** — Node.js · Express · Socket.IO · REST APIs · JWT · Zod

**Data & AI** — MongoDB · Redis · Pinecone · Supabase (Postgres) · Drift · LLM APIs (Groq, Gemini) · RAG · Vector search · STT/TTS

**Real-time & Media** — WebSockets · WebRTC · LiveKit · Redis Pub/Sub · Streaming pipelines

**Infrastructure & Tools** — Docker · Docker Compose · Nginx · Git & GitHub · Vercel · Render · Linux (Arch, Hyprland)

## Currently Working On

- Improving WebChat's real-time communication and community experience.
- Refining ARC-AI's voice interaction, tool execution, and runtime reliability.
- Practising data structures and algorithms in **C++** with documented notes, alongside learning **Python**.
- Strengthening how I explain approaches, analyze complexity, debug problems, and communicate technical ideas.

<a href="https://github.com/Aashutosh31/algorithmic-thinking"><img src="https://img.shields.io/badge/DSA%20Notes-algorithmic--thinking-1a1b26?style=flat-square&logo=cplusplus&logoColor=7aa2f7" alt="DSA notes" /></a>

### Beyond Building Projects

I'm deliberately working on three complementary areas:

1. **Building production-style projects** and understanding the real engineering trade-offs behind them.
2. **Practising algorithms and problem-solving** to get stronger for technical interviews.
3. **Improving technical communication** — presenting projects, explaining decisions, and reasoning through unfamiliar problems.

---

## GitHub Activity

<div align="center">

<a href="https://github.com/Aashutosh31"><img height="165" src="https://github-readme-stats.vercel.app/api?username=Aashutosh31&show_icons=true&hide=contribs&theme=tokyonight&hide_border=true&bg_color=1a1b26&title_color=7aa2f7&icon_color=bb9af7&text_color=c0caf5&ring_color=7dcfff" alt="Aashutosh31's GitHub stats" /></a>
<a href="https://github.com/Aashutosh31"><img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Aashutosh31&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=1a1b26&title_color=7aa2f7&text_color=c0caf5" alt="Aashutosh31's top languages" /></a>

<a href="https://github.com/Aashutosh31"><img src="https://streak-stats.demolab.com?user=Aashutosh31&theme=tokyonight&hide_border=true&background=1a1b26&ring=7aa2f7&fire=bb9af7&currStreakLabel=7dcfff&sideLabels=c0caf5&dates=a9b1d6&currStreakNum=c0caf5&sideNums=c0caf5" alt="Aashutosh31's contribution streak" /></a>

</div>

## Connect

- **Portfolio:** [aashutoshbairagi.vercel.app](https://aashutoshbairagi.vercel.app/)
- **GitHub:** [github.com/Aashutosh31](https://github.com/Aashutosh31)
- **LinkedIn:** [Aashutosh Bairagi](https://www.linkedin.com/in/aashutosh-bairagi-559aa530b/)
- **X:** [@Aashutosh_dev31](https://x.com/Aashutosh_dev31)

<div align="center">
  <img src="assets/footer.svg" alt="Build, debug, understand, improve." width="100%" />
</div>
