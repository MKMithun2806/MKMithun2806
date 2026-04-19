<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=VT323&size=65&pause=1200&color=00ff88&background=000000&center=true&vCenter=true&width=880&height=120&lines=%3CRed+Team+Aspirant+/%3E;%3CInfrastructure+Engineer+/%3E;%3COffensive+Security+/%3E;%3CCloud+stuff+/%3E;%3CAI-Augmented+Builder+/%3E" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=MKMithun2806&color=00ff88&style=flat-square">
  <img src="https://img.shields.io/github/followers/MKMithun2806?style=flat-square&color=00ff88">
</p>

<br />

<p align="center">
I build systems that <b>observe, analyze, and act</b>.
</p>

<p align="center">
Offensive security meets cloud-native engineering — designing recon pipelines, private infrastructure, and AI-powered tooling.
</p>

<br>

---

<h2 align="center">⚡ Core Stack</h2>

<h3 align="center">Infrastructure</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=linux,docker,aws,kubernetes,nginx,raspberrypi" />
  <br/>
  <img src="https://img.shields.io/badge/n8n-Workflow%20Automation-00ff88?style=flat-square" />
  <img src="https://img.shields.io/badge/OpenWrt-Router%20OS-00ff88?style=flat-square&logo=openwrt&logoColor=black" />
  <img src="https://img.shields.io/badge/pfSense-Firewall-00ff88?style=flat-square&logo=pfsense&logoColor=black" />
</p>

<h3 align="center">Development</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,bash,js,powershell,git" />
  <p align="center">
  <img src="https://img.shields.io/badge/Claude-Code-00ff88?style=flat-square&logo=anthropic&logoColor=black" />
  <img src="https://img.shields.io/badge/Gemini-CLI-00ff88?style=flat-square&logo=google-gemini&logoColor=black" />
  <img src="https://img.shields.io/badge/Cursor-AI%20Editor-00ff88?style=flat-square&logo=cursor&logoColor=black" />
</p>
</p>
<h3 align="center">Network & Control Plane</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=grafana,prometheus,arch" />
  <br/><br/>
  <img src="https://img.shields.io/badge/Tailscale-Mesh%20VPN-00ff88?style=flat-square&logo=tailscale&logoColor=black" />
  <img src="https://img.shields.io/badge/Proxmox-VE-E57000?style=flat-square&logo=proxmox&logoColor=white" />
  <img src="https://img.shields.io/badge/Kali-Linux-557C94?style=flat-square&logo=kalilinux&logoColor=white" />
</p>
<br>

---

<h2 align="center">💀 Offensive Profile</h2>

```bash
mitch@watchdog:~$ whoami
ROLE        : Red Team Aspirant
FOCUS       : Internal Networks / Infrastructure / Physical Security
INTEREST    : Recon automation, attack simulation, lab-built tooling
STYLE       : Build systems that scale offensive work

mitch@watchdog:~$ tools --stack

Recon       : subfinder, naabu, httpx, nuclei, nmap, amass
Wireless    : aircrack-ng, hashcat, tcpdump, wireshark
Exploitation: metasploit, custom payloads
Infra       : n8n, docker, tailscale, proxmox, swarm

mitch@watchdog:~$ echo $CURRENT_OBJECTIVE
"Build scalable offensive infrastructure and grow into a real Red Team operator"

mitch@watchdog:~$ echo $PHILOSOPHY
"I actually have to know the infrastructure to break it"
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

# 🔮 Future Architecture (The Dream Setup)

```mermaid
flowchart TB
    subgraph Edge["Edge Network & Security"]
        ISP([Internet])
        UDM[Ubiquiti Dream Machine / EdgeRouter]
        FW[Advanced Firewall Rules / IDS]
        ISP --> UDM
        UDM --> FW
    end

    subgraph Proxmox_Cluster["Proxmox VE HA Cluster (The Beast)"]
        direction TB
        PVE1[Proxmox Node 1]
        PVE2[Proxmox Node 2]
        PVE3[Proxmox Node 3]
        CEPH_OSD1[(OSD Pool 1)]
        CEPH_OSD2[(OSD Pool 2)]
        CEPH_OSD3[(OSD Pool 3)]
        PVE1 <--> CEPH_OSD1
        PVE2 <--> CEPH_OSD2
        PVE3 <--> CEPH_OSD3
    end

    subgraph K3s_Grid["Kubernetes Control Plane"]
        K3S_M1[K3s Master 1]
        K3S_M2[K3s Master 2]
        K3S_W1[K3s Worker 1]
        K3S_W2[K3s Worker 2]
        K3S_W3[K3s Worker 3]
    end

    FW --> PVE1
    FW --> PVE2
    FW --> PVE3

    PVE1 --- K3S_M1
    PVE2 --- K3S_M2
    PVE3 --- K3S_W1
    PVE1 --- K3S_W2
    PVE2 --- K3S_W3

    subgraph Cloud_Ext["Cloud Extensions"]
        ORACLE[Oracle Cloud A1 - Backup Node]
        RPI[Raspberry Pi - Satellite]
    end

    FW <--> ORACLE
    FW <--> RPI

    subgraph Services["High-Availability Services"]
        N8N_HA[n8n Cluster]
        GITEA_HA[Gitea HA]
        MON[Prometheus + Grafana + Loki]
        AI[MCP Servers / LLM Inference]
    end

    K3s_Grid --> Services
```

# 🏠 Current Architecture

```mermaid
flowchart TB
    subgraph Clients
    A[Home Devices]
    B[Studio Devices]
    end
    subgraph Network_Fabric["Tailscale Mesh (The Glue)"]
    TS[Tailscale VPN]
    SWARM_NET[Docker Overlay Network]
    DNS[Pi-hole DNS]
    end
    A --> TS
    B --> TS
    TS --> DNS
    subgraph OpenClaw_EC2["OpenClaw EC2 (The Brain)"]
        EC2_AWS["AWS t4g.small"]
        subgraph OPENCLAW_CORE[OpenClaw Core]
            OC_GATEWAY[Gateway]
            OC_AGENT[Steve The Agent]
            OC_SKILLS[Skills & Tools]
        end
        subgraph EC2_SERVICES[Services]
            N8N_EC2[n8n]
            GITEA_EC2[Gitea]
            SILVER_EC2[SilverBullet]
        end
    end
    subgraph Raspberry_Pi["Raspberry Pi (Home Muscle)"]
        subgraph PI_CORE[Pi Core]
            PI_DOCKER[Docker/Podman]
            PI_TAIL[Tailscale Client]
        end
        subgraph HOME_SERVICES[Local Ops]
            JELLY[Jellyfin]
            NAVI[Navidrome]
            WATCHDOG[Watchdog UI]
            GRAFANA[Prometheus + Grafana]
        end
        subgraph PI_STORAGE[Local Storage]
            NAS_1TB[/"1TB Local NAS"/]
        end
    end
    subgraph Windows_Studio["Windows 10 Studio (The Vault)"]
        WIN_DESK[Desktop Environment]
        subgraph WIN_STORAGE[Studio NAS]
            WIN_NAS[/"Large Media & Vault Storage"/]
        end
        subgraph DEV_TOOLS[Dev Environment]
            VS_CODE[VS Code / Cursor]
            TERM[Terminal / WSL]
        end
    end
    %% Connections
    TS --> SWARM_NET
    SWARM_NET --> EC2_AWS
    SWARM_NET --> PI_DOCKER
    SWARM_NET --> WIN_DESK
    OC_AGENT -.->|Controls| PI_DOCKER
    OC_AGENT -.->|Manages| WIN_DESK
    WIN_NAS <-->|Sync| NAS_1TB
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

OpenClaw Setup:
- "Steve" (The Agent): Running on AWS EC2 t4g.small
- Role: Personal infrastructure assistant & automation engine
- Capabilities: 
  - GitHub management (PRs, Issues, Commits)
  - Infrastructure monitoring & health checks
  - Automated email & calendar management
  - Slack/Telegram integration for real-time updates
- Philosophy: AI doesn't replace engineering. It amplifies it.
```
---
<h2 align="center">🎯 Red Team Direction</h2> <p align="center"> Focused on learning offensive tradecraft, internal network testing, and building lab environments that simulate real targets. </p> <p align="center"> The goal is not just to use tools it is to understand systems deeply enough to break them. </p>

---

<h2 align="center">📊 GitHub Metrics</h2>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=MKMithun2806&background=0D1117&border=00ff88&stroke=00ff88&ring=00ff88&fire=00ff88&currStreakLabel=00ff88&sideLabels=C9D1D9&currStreakNum=C9D1D9&dates=8B949E&sideNums=C9D1D9" height="165"/>
</p>

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

# If u Plan on stalking me
*im 14*
*i really need a server computer or rack to use proxmox on smth othern then in VMware😭😭*

*Built. Broken. Documented.*

[🧠 About me](https://github.com/MKMithun2806/MKMithun2806/blob/main/Aboutme.md)

[🔴 Security Reports (Real Exploits & Findings)](https://github.com/MKMithun2806/Security-Reports)

[⚙️ Homelab Deep Dive](https://github.com/MKMithun2806/MKMithun2806/blob/main/Homelab-docs.md)

<img width="1121" height="713" alt="image" src="https://github.com/user-attachments/assets/623224bf-4367-414f-88af-123dc084cfb2" />
