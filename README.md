<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7aa2f7,100:bb9af7&height=180&section=header&text=Aashutosh%20Bairagi&fontSize=46&fontColor=1a1b26&fontAlignY=38&animation=fadeIn&desc=Full-Stack%20Developer%20%7C%20Arch%20Linux%20%7C%20VS%20Code&descAlignY=58&descSize=18&descColor=1a1b26" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=24&duration=2800&pause=1200&color=7AA2F7&center=true&vCenter=true&width=650&lines=whoami+%3E%3E+Aashutosh+Bairagi;Building+real-time+systems+%26+AI+agents;ARC-AI+%2B+WebChat;Arch+Linux+%7C+Hyprland+%7C+VS+Code" alt="Typing SVG" />

<br/>

<img src="https://img.shields.io/badge/OS-Arch_Linux-1a1b26?style=for-the-badge&logo=archlinux&logoColor=7aa2f7&labelColor=1a1b26" />
<img src="https://img.shields.io/badge/WM-Hyprland-1a1b26?style=for-the-badge&logo=wayland&logoColor=bb9af7&labelColor=1a1b26" />
<img src="https://img.shields.io/badge/status-shipping-1a1b26?style=for-the-badge&logo=girlsreunited&logoColor=9ece6a&labelColor=1a1b26" />
<img src="https://komarev.com/ghpvc/?username=Aashutosh31&style=for-the-badge&color=1a1b26&label=PROFILE+VIEWS&labelColor=1a1b26" />

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1a1b26,100:1a1b26&height=2" width="100%"/>

```
┌──(aashutosh㉿arch)-[~/introduction]
└─$ cat about.md
```

> 🚀 **2nd Year CS Student · Building distributed real-time applications and AI systems**
> Creator of **ARC-AI** and **WebChat** — real-time messaging, voice/video
> infrastructure, and autonomous agent tooling, built end-to-end: architecture, backend,
> and deployment.

<div align="center">

[![Portfolio](https://img.shields.io/badge/Portfolio-aashutoshbairagi.vercel.app-1a1b26?style=for-the-badge&logo=vercel&logoColor=c0caf5&labelColor=1a1b26)](https://aashutoshbairagi.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Aashutosh_Bairagi-1a1b26?style=for-the-badge&logo=linkedin&logoColor=7aa2f7&labelColor=1a1b26)](https://www.linkedin.com/in/aashutosh-bairagi-559aa530b/)

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1a1b26,100:1a1b26&height=2" width="100%"/>

## 🧠 Featured Projects

```
┌──(aashutosh㉿arch)-[~/projects]
└─$ tree -L 1 --color=tokyonight
```

<table>
<tr>
<td width="50%" valign="top">

### 🌐 WebChat
**Distributed Real-Time Communication Platform**

![Blue](https://img.shields.io/badge/-Real--time%20Mesh-24283b?style=flat-square&labelColor=24283b&color=7aa2f7)

A multi-paradigm social platform merging low-latency persistent messaging, Discord-style communities, Reddit-style forums, and ephemeral social feeds into one ecosystem.

**Built solo:** architecture, backend, real-time infrastructure, authentication, and deployment.

<details>
<summary><b>⚡ Engineering Highlights</b></summary>
<br/>

- **Redis Pub/Sub** keeps WebSocket message delivery synchronized across multiple server instances, so real-time events stay consistent as the backend scales horizontally
- **LiveKit** powers multi-party WebRTC voice/video rooms, offloading media routing away from the application server
- Payload encryption via the native **Web Crypto API**, paired with short-lived JWT access tokens and rotating refresh tokens, to limit exposure from a compromised session
- Embedded **ARC Assistant** (Mistral AI + Pinecone vector memory) surfaces contextual support inside communities without a separate lookup step
- Dockerized multi-container setup separates the API, real-time layer, and datastores into independently deployable services

</details>

`React` `Node.js` `MongoDB` `Redis` `Socket.IO` `LiveKit` `Tailwind` `Docker`

[![Repo](https://img.shields.io/badge/Architecture_&_Docs-1a1b26?style=for-the-badge&logo=github&logoColor=7aa2f7&labelColor=1a1b26)](https://github.com/Aashutosh31/webchat-system-design)
[![Live](https://img.shields.io/badge/Live_Production-1a1b26?style=for-the-badge&logo=vercel&logoColor=7aa2f7&labelColor=1a1b26)](https://webchat.qzz.io)

</td>
<td width="50%" valign="top">

### 🤖 ARC-AI
**Real-Time AI Assistant with Streaming Voice & Long-Term Memory**

![Violet](https://img.shields.io/badge/-RAG%20Memory-24283b?style=flat-square&labelColor=24283b&color=bb9af7)

An AI agent that streams responses, executes tools, and maintains long-term memory — built on a full MERN-stack execution core.

**Built solo:** architecture, backend, agent runtime, RAG pipeline, and UI actuation.

<details>
<summary><b>⚡ Engineering Highlights</b></summary>
<br/>

- Token-by-token **WebSocket** streaming renders responses as they're generated instead of waiting for the full completion
- Voice responses are interruptible — a buffered TTS pipeline stops playback mid-sentence once the user starts speaking
- **RAG-based memory** retrieves relevant Pinecone embeddings from past conversations instead of replaying full history on every turn
- Multi-step tool execution (web search, external APIs) runs without requiring a new prompt for each step
- Recovery/retry logic sits above the LLM provider layer, so a failed call doesn't break `tool_call` continuity mid-execution

</details>

`React` `Node.js` `WebSockets` `Vector DB` `TTS/STT` `RAG`

[![Repo](https://img.shields.io/badge/GitHub-1a1b26?style=for-the-badge&logo=github&logoColor=bb9af7&labelColor=1a1b26)](https://github.com/Aashutosh31/arc-ai-project)
[![Live](https://img.shields.io/badge/Live_Demo-1a1b26?style=for-the-badge&logo=vercel&logoColor=bb9af7&labelColor=1a1b26)](https://arc-ai-project.vercel.app)

</td>
</tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1a1b26,100:1a1b26&height=2" width="100%"/>

## 🧩 Engineering Challenges

```
┌──(aashutosh㉿arch)-[~/challenges]
└─$ git log --oneline --grep="fix\|solve"
```

* Synchronized real-time events across multiple server instances using Redis Pub/Sub, avoiding the single-instance WebSocket bottleneck
* Built an interruptible TTS playback pipeline so voice responses can be cut off mid-sentence without breaking the buffering logic
* Designed a semantic memory layer with Pinecone embeddings so the agent recalls relevant context instead of replaying full conversation history
* Separated recovery/retry logic above the LLM provider layer in ARC-AI, preserving streaming continuity and `tool_call` consistency when a request fails
* Containerized the full stack (API, real-time layer, datastores) with Docker for consistent local and production environments

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1a1b26,100:1a1b26&height=2" width="100%"/>

## ⚙️ What I Work On

```
┌──(aashutosh㉿arch)-[~/skills]
└─$ fastfetch --focus
```

<table>
<tr><td width="140">🧠 <b>AI Agents</b></td><td>LLMs, RAG, semantic memory, tool calling</td></tr>
<tr><td>⚡ <b>Real-Time</b></td><td>WebSockets, WebRTC, streaming architectures, low-latency sync</td></tr>
<tr><td>🛠 <b>Backend</b></td><td>Node.js, distributed system patterns, database optimization</td></tr>
<tr><td>📦 <b>DevOps</b></td><td>Git workflows, Docker orchestration, CI/CD</td></tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1a1b26,100:1a1b26&height=2" width="100%"/>

## 🛠 Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=react,tailwind,redux,nodejs,express,socketio,mongodb,redis,docker,vercel,git,github,linux,arch,vscode,ts&theme=dark" />

</div>

<br/>

<table align="center">
<tr><td>🎨 <b>Frontend</b></td><td>React · Tailwind CSS · Framer Motion · Zustand</td></tr>
<tr><td>🧩 <b>Backend</b></td><td>Node.js · Express · Socket.IO</td></tr>
<tr><td>🗄️ <b>Data & Cache</b></td><td>MongoDB · Redis · Pinecone (Vector DB)</td></tr>
<tr><td>☁️ <b>Infra</b></td><td>Docker · LiveKit (WebRTC) · Vercel · Render</td></tr>
<tr><td>💻 <b>Daily Driver</b></td><td>Arch Linux · Hyprland · Omarchy · VS Code</td></tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1a1b26,100:1a1b26&height=2" width="100%"/>

## 📌 Currently

```diff
+ Scaling WebChat infrastructure and expanding community features
+ Building and refining autonomous AI agents
+ Contributing to open-source workflows
+ Tuning the Hyprland rice, one pixel at a time
```

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1a1b26,100:1a1b26&height=2" width="100%"/>

## 📊 Activity & Languages

<div align="center">

<img height="165" src="https://github-stats-extended.vercel.app/api?username=Aashutosh31&show_icons=true&theme=tokyonight&hide_border=true&bg_color=1a1b26&title_color=7aa2f7&icon_color=bb9af7&text_color=c0caf5" />
<img height="165" src="https://github-stats-extended.vercel.app/api/top-langs/?username=Aashutosh31&layout=compact&theme=tokyonight&hide_border=true&bg_color=1a1b26&title_color=7aa2f7&text_color=c0caf5" />

<br/>
<img src="https://github-readme-activity-graph.vercel.app/graph?username=Aashutosh31&theme=tokyo-night&hide_border=true&bg_color=1a1b26&color=7aa2f7&line=bb9af7&point=c0caf5" width="100%"/>

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:1a1b26,100:1a1b26&height=2" width="100%"/>

## 📫 Reach Me

<div align="center">

[![Portfolio](https://img.shields.io/badge/Portfolio-7aa2f7?style=for-the-badge&logo=firefox&logoColor=1a1b26)](https://aashutoshbairagi.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-bb9af7?style=for-the-badge&logo=linkedin&logoColor=1a1b26)](https://www.linkedin.com/in/aashutosh-bairagi-559aa530b/)
[![GitHub](https://img.shields.io/badge/GitHub-c0caf5?style=for-the-badge&logo=github&logoColor=1a1b26)](https://github.com/Aashutosh31)

</div>

<br/>

<div align="center">

```
┌──(aashutosh㉿arch)-[~]
└─$ exit
```

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:bb9af7,100:7aa2f7&height=120&section=footer"/>

</div>
