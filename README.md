<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=VT323&size=65&pause=1200&color=00ff88&background=000000&center=true&vCenter=true&width=880&height=120&lines=%3CRed+Team+Operator+/%3E;%3CInfrastructure+Engineer+/%3E;%3COffensive+Security+/%3E;%3CCloud+Systems+/%3E;%3CAI-Augmented+Builder+/%3E" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=MKMithun2806&color=00ff88&style=flat-square">
  <img src="https://img.shields.io/github/followers/MKMithun2806?style=flat-square&color=00ff88">
</p>

<br />

<p align="center">
I build systems that <b>observe, analyze, and scale</b>.
</p>

<p align="center">
Offensive security meets cloud-native engineering — designing recon pipelines, private infrastructure, and AI-powered tooling.
</p>

<br>

---

<h2 align="center">⚡ Core Stack</h2>

<h3 align="center">Infrastructure</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=linux,docker,aws,cloudflare,nginx,raspberrypi" />
  <br/>
  <img src="https://img.shields.io/badge/n8n-Workflow%20Automation-00ff88?style=flat-square" />
</p>

<h3 align="center">Development</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,bash,js,ts" />
</p>

<h3 align="center">Observability & Control</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=grafana,prometheus" />
</p>

<br>

---

<h2 align="center">💀 Offensive Profile</h2>

```bash
mitch@watchdog:~$ whoami
FUll INFO.  : [Github Whoami](https://github.com/MKMithun2806/MKMithun2806/blob/main/Aboutme.md)
ROLE        : Red Team Aspirant
FOCUS       : Systems / Network / Physical Security
INTEREST    : Breaking infrastructure > web apps

mitch@watchdog:~$ tools --stack
Recon       : subfinder, naabu, httpx, nuclei, nmap, amass
Wireless    : aircrack-ng, hashcat, tcpdump, wireshark
Exploitation: metasploit, custom payloads
Infra       : n8n, docker, tailscale, proxmox

mitch@watchdog:~$ echo $CURRENT_OBJECTIVE
"Build scalable offensive infrastructure and operate as a Red Team Operator"

mitch@watchdog:~$ sudo access system
access granted: keep going.
```

---

<h2 align="center">🛰️ Flagship Project — Watchdog</h2>

<p align="center">
Hardware-triggered, cloud-native reconnaissance platform.
</p>

<p align="center">
Flipper Zero → ESP32 → n8n → Cloud Recon Workers → AI Analysis → Streamlit UI
</p>

---

<h2 align="center">⚙️ Infrastructure Ecosystem</h2>

```mermaid
flowchart TB

%% ================= CLIENT LAYER =================
subgraph Clients
    U1[Operator Dashboard]
    U2[AI Interfaces / MCP Clients]
end

%% ================= NETWORK =================
subgraph Network
    TS[Tailscale Mesh VPN]
end

U1 --> TS
U2 --> TS

%% ================= CONTROL LAYER =================
subgraph Control["Raspberry Pi (Control Plane)"]

    N8N[n8n Orchestrator]
    WATCH[Watchdog UI]
    MCP_LOCAL[Local MCP Gateway]

end

TS --> N8N
TS --> WATCH
TS --> MCP_LOCAL

%% ================= OROX CLUSTER =================
subgraph OROX["Oryx Mix Cluster (Proxmox HA - Planned)"]

    subgraph Compute
        VM1[Recon Workers]
        VM2[Service Nodes]
        VM3[Internal Tooling]
    end

    subgraph Storage
        NAS[Distributed Storage / Backups]
    end

    VM1 --> NAS
    VM2 --> NAS
    VM3 --> NAS

end

N8N --> VM1
WATCH --> VM2

%% ================= OCI AMPERE =================
subgraph OCI["Oracle Cloud - Ampere A1 (Tailnet Integrated)"]

    MCP_AI[MCP Servers]
    AI_HOST[AI Hosting / LLM Inference]
    MC[Minecraft Servers]

end

N8N --> MCP_AI
MCP_LOCAL --> MCP_AI

%% ================= AWS =================
subgraph AWS["AWS EC2"]

    MCP1[Dedicated MCP Servers]
    MCP2[Tool Execution Nodes]
    RECON[Ephemeral Recon Instances]

end

N8N --> RECON
MCP_LOCAL --> MCP1
MCP_LOCAL --> MCP2

%% ================= DATA FLOW =================
subgraph Data
    S3[Amazon S3]
    PI_STORAGE[Local Pi Storage]
end

RECON --> S3
VM1 --> PI_STORAGE
AI_HOST --> PI_STORAGE
```
---

<h2 align="center">🤖 AI-Augmented Development</h2>

<p align="center">
AI is not a chatbot — it's part of the system.
</p>

```bash
Workflow:
- Architecture design with AI
- Rapid infra scripting (Bash / Python)
- MCP servers for tool integration
- Automated recon + analysis pipelines

Philosophy:
AI doesn't replace engineering.
It amplifies it.
```

---

<h2 align="center">📊 GitHub Metrics</h2>

<p align="center">
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=MKMithun2806&show_icons=true&bg_color=0d1117&title_color=00ff88&text_color=c9d1d9&icon_color=00ff88&border_color=00ff88" height="165"/>
  
  <img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=MKMithun2806&layout=compact&bg_color=0d1117&title_color=00ff88&text_color=c9d1d9&border_color=00ff88" height="165"/>
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=MKMithun2806&background=0D1117&border=00ff88&stroke=00ff88&ring=00ff88&fire=00ff88&currStreakLabel=00ff88&sideLabels=C9D1D9&currStreakNum=C9D1D9&dates=8B949E&sideNums=C9D1D9" height="165"/>
</p>

---

<h2 align="center">📡 Activity</h2>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=MKMithun2806&theme=chartreuse-dark&hide_border=true"/>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/MKMithun2806/MKMithun2806/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/MKMithun2806/MKMithun2806/output/github-snake.svg" />
    <img alt="github contribution snake" src="https://raw.githubusercontent.com/MKMithun2806/MKMithun2806/output/github-snake-dark.svg" />
  </picture>
</p>

---

<h2 align="center">🚀 Philosophy</h2>

<p align="center">
I don't build apps. I build systems.
</p>

<p align="center">
<b>Build infrastructure that sees everything — so nothing goes unnoticed.</b>
</p>
