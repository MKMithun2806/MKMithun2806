The Funny Part

This incident was especially deceptive because every piece of evidence initially pointed somewhere else.

Evidence suggesting Wi-Fi

High latency to router
100-400ms ping times
Internet completely dead

Conclusion:

"Maybe the Qualcomm Wi-Fi card is dying."

Result:

Wrong.

---

Evidence suggesting firmware

ath10k driver
QCA9377 chipset
Various firmware messages in dmesg

Conclusion:

"Maybe ath10k firmware is broken."

Result:

Wrong.

---

Evidence suggesting MTU problems

HTTPS hangs
Docker pulls timeout
Tailscale interface present

Conclusion:

"Maybe PMTU discovery is broken."

Result:

Wrong.

---

Evidence suggesting DNS problems

Docker unable to pull images
External services unreachable

Conclusion:

"Maybe DNS is broken."

Result:

Wrong.

DNS worked.

---

Evidence suggesting firewall issues

nftables rules
iptables rules
Tailscale chains
Docker chains

Conclusion:

"Some firewall rule is dropping traffic."

Result:

Wrong.

Flushing nftables and iptables changed nothing.

---

Evidence suggesting Docker issues

docker pull timeouts
docker compose failures

Conclusion:

"Docker is broken."

Result:

Wrong.

Docker was innocent.

---

Evidence suggesting router issues

Internet unreachable
Traceroute fails

Conclusion:

"Router is broken."

Result:

Wrong.

Router responded perfectly.

---

Evidence suggesting Ethernet issues

After switching from Wi-Fi to Ethernet:

Problem still exists

Conclusion:

"Maybe the Ethernet port is broken."

Result:

Wrong.

---

The Clue Nobody Notices

One observation never fit any theory:

ARP to router: ~0.5ms
Ping to router: 100-400ms

Layer 2 was perfect.

Layer 3 was nonsense.

That combination is extremely suspicious.

---

The Plot Twist

Every subsystem appeared guilty:

- Wi-Fi
- Ethernet
- Docker
- DNS
- MTU
- Router
- Firmware
- nftables
- iptables

Yet every test slowly eliminated them.

The investigation kept narrowing until only one suspect remained:

Tailscale policy routing

And when route acceptance was disabled:

sudo tailscale set --accept-routes=false

Every symptom disappeared immediately.

Internet restored.
Docker restored.
Latency restored.
Sanity restored.

The entire outage was caused by a single route:

192.168.1.0/24 via tailscale0

advertised by MKS and accepted by Alpine-Node.

A one-line route entry managed to impersonate half a dozen unrelated networking failures.
