# 👋 Sup, I'm Mithun Krish
You can call me Mitch 

### 🛰️ Developer of Random things • Red Team Aspirant • Systems & Infrastructure Specialist

I design systems that **observe, analyze, and scale**. My work sits at the intersection of **offensive security research and cloud-native engineering**, focusing on building high-performance scanning pipelines and resilient private infrastructure. 

**My ultimate goal is to operate as a Red Team Operator.** I focus on the foundation—systems, networks, and physical security. **I'm not interested in web hacking;** I'd rather crack a system shell or bypass a physical lock than hunt for bugs in a web form.

---

### Featured Project: Watchdog 🐕‍🦺

Hardware-Triggered, Cloud-Native Reconnaissance Platform

I built an end-to-end offensive security platform that bridges physical hardware with scalable cloud infrastructure, enabling one-tap reconnaissance deployments from a handheld device.

⸻

⚡ Architecture Overview

🔘 Edge Trigger Layer
A custom JavaScript application running on the Flipper Zero communicates over serial with an ESP32, acting as a wireless bridge to initiate remote scan workflows.

☁️ Orchestration Layer
Workflows are coordinated using n8n, which dynamically provisions pre-configured Amazon EC2 instances (Golden AMIs) for distributed, high-performance reconnaissance.

⚔️ Execution Layer
Ephemeral cloud instances execute automated recon pipelines (service enumeration, vulnerability detection, and attack path modeling), then self-terminate to optimize cost and operational hygiene.

📦 Data Pipeline
Scan artifacts are:
	•	Synced to Amazon S3 for persistence
	•	Mirrored to a local Raspberry Pi NAS for offline access
	•	Automatically cleaned up to maintain a minimal cloud footprint

🧠 Intelligence Layer
Custom AI-driven analysis processes raw recon output to:
	•	Extract high-signal vulnerabilities
	•	Generate realistic attack paths
	•	Prioritize findings based on exploitability

📊 Visualization Layer
A custom-built Streamlit dashboard provides:
	•	Real-time scan control and monitoring
	•	Interactive report exploration
	•	Payload generation and operator tooling

---

# 💀 Offensive Capabilities

### 🖥️ System Exploitation & Persistence
- **Shells & Payloads:** Experienced in weaponizing reverse shells and establishing persistent backdoors.
- **Privilege Escalation:** Manual and automated PrivEsc on Linux and Windows environments to reach Root/SYSTEM.
- **C2 & AD:** Actively learning and deploying Command & Control frameworks and Active Directory exploitation (Kerberoasting, Lateral Movement).

### 📶 WiFi & Network Domination
- **Wireless Exploitation:** Strong hands-on experience with **802.11 exploitation**, Hashcat-based WPA/WPA2 cracking, and PCAP surgical analysis.
- **Network Manipulation:** Proficient in DNS Spoofing, ARP Poisoning, and complex MITM attacks.
- **Access Points:** Deploying Evil Portals and Rogue APs for credential harvesting.

### 🛡️ Physical Penetration Testing (Interest)
- **Physical Security:** Exploring the art of physical bypass, social engineering, and the intersection of hardware and physical entry.

### 📝 Vulnerability Reporting & Documentation
- **Professional Deliverables:** Proficient in translating technical exploits into industry-standard vulnerability reports.
- **Risk Assessment:** Familiar with **PTES methodology** and **CVSS-style risk matrices** to accurately categorize findings.
- **Live Documentation:** [Security-Reports Repository](https://github.com/MKMithun2806/Security-Reports)

---

# ⚙️ Infrastructure Ecosystem

### ☁️ Multi-Cloud Scanning Lab (The Workers)
A distributed cloud footprint used for reconnaissance workloads and security research.
- **Oracle Cloud (OCI):** 24GB RAM ARM instances for heavy lifting.
- **AWS:** Elastic workloads for specialized, high-intensity recon tasks.
- **Tailscale:** A private mesh network (Tailnet) connecting cloud workers to the local control layer.

### 🖥️ Homelab (The Control Layer)
A high-density **Raspberry Pi 4 (8GB)** environment running a 17-container stack. This serves as the brain for my reconnaissance pipelines and local observability.
- **Networking Depth:** Deep-diving into L2/L3 protocols. I have a strong grasp of networking fundamentals, but I recognize that true mastery is a lifelong pursuit—especially in the complex world of distributed systems.
- **Observability:** Prometheus, Grafana, and Node Exporter.
- **Security & Recon:** NetAlertX, Pi-hole, and n8n (Workflow engine).
- **Development:** Gitea (Local Git), Code-Server (Remote VS Code), and Portainer.

### 🐳 Docker & Containerization
Deep hands-on experience designing and managing multi-container environments on ARM64 and cloud infrastructure.
- **Compose Stacks:** Authoring and maintaining complex `docker-compose` stacks (17+ containers).
- **ARM64 Builds:** Cross-platform image selection and custom builds targeting ARM64 architecture.
- **Security-focused deployments:** Containerizing offensive security tools (Subfinder, Naabu, HTTPX, Nuclei, Nmap, Katana, GAU, Amass) as isolated pipeline workers.

### 🔌 MCP Server Development
Experienced in building and deploying **Model Context Protocol (MCP) servers** to extend AI assistants with custom tooling.
- **Custom MCP Architecture:** Designing tool schemas, handlers, and transport layers (stdio / SSE) from scratch.
- **Security Tooling Integration:** Bridging offensive recon tools and pipeline data into LLM-accessible interfaces.
- **Self-Hosted Deployment:** Running MCP servers on Raspberry Pi / Ubuntu ARM64 integrated with Ollama backends.

---

# 🧪 Current Experiments & Learning Path

- **VDP Roadmap:** Currently focusing on my board exams, with plans to transition into active Bug Bounty hunting once I turn 15 and the academic season concludes.
- **Advanced C2:** Researching stealthy communication channels for C2 traffic.
- **Active Directory Lab:** Building internal AD environments to practice bloodhound analysis and group policy exploitation.
  

---

# 💻 Hardware

- **Daily Driver:** ASUS ROG Zephyrus G16 (Intel Core Ultra 9 | RTX 4070)
- **The Brain:** Raspberry Pi 4 (8GB) - The 24/7 infrastructure controller.
- **Tools:** Flipper Zero + ESP32 WiFi Dev Board, RTL-SDR, and various wireless adapters.

---

# 🚀 Philosophy

I don't care about "smart homes." I care about **intelligent infrastructure**. 

> Build systems that see everything, so nothing goes unpatched.

---

# 🤖 AI-Augmented Development
I build software using AI-assisted development workflows, focusing on rapid infrastructure tooling, automation, and experimental security systems. Rather than treating AI as a chatbot, I use it as an engineering copilot for building real systems.

### Development Workflow
* **AI Pair Programming:** Using models like Claude for architecture design, debugging, and rapid prototyping.
* **Infrastructure Code:** Generating and refining Bash, Python, and Docker tooling for distributed scanning systems.
* **Rapid Iteration:** Building experimental security tools in hours instead of days through AI-assisted development cycles.
* **Toolchain Integration:** Connecting AI models to infrastructure through **MCP servers** and automation pipelines.

### Things I Build with AI
* **Recon Orchestration Pipelines:** Custom infrastructure automation scripts.
* **Security Analysis Tools:** LLM-powered scan summarization systems.
* **Custom WebUIs:** Developing bespoke chatbot interfaces and dashboards for internal tool management.
* **AI-Assisted Threat Analysis:** Automated workflows for real-time intel gathering.

### Philosophy
> AI doesn’t replace engineering — it amplifies it. The real skill is knowing what to build, how systems should behave, and using AI to move from idea → working system extremely quickly.

---

# 🎮 Beyond the Terminal

When the monitors are off, I'm usually in high-mobility FPS or immersive story-driven worlds.
- **Favs:** DOOM Eternal, Titanfall 2, Halo Infinite, Crysis, Battlefield 6, Valorant, Batman Trilogy, Ghost of Tsushima, All AC Games ,etc
- **Books:** Reading Art Of Deceptioon rn
- Im also a cinephile
My favorites are; The Space Odyssey, Interstellar, and inception
If we talk TV shows i like; Peaky Blinders, Stranger Things and Mr.Robot
