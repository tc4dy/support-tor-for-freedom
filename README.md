<div align="center">

<pre>
  ████████╗ ██████╗ ██████╗     ███████╗██╗   ██╗██████╗ ██████╗  ██████╗ ██████╗ ████████╗
   ╚══██╔══╝██╔═══██╗██╔══██╗    ██╔════╝██║   ██║██╔══██╗██╔══██╗██╔═══██╗██╔══██╗╚══██╔══╝
   ██║   ██║   ██║██████╔╝    ███████╗██║   ██║██████╔╝██████╔╝██║   ██║██████╔╝   ██║
   ██║   ██║   ██║██╔══██╗    ╚════██║██║   ██║██╔═══╝ ██╔═══╝ ██║   ██║██╔══██╗   ██║
   ██║   ╚██████╔╝██║  ██║    ███████║╚██████╔╝██║     ██║     ╚██████╔╝██║  ██║   ██║
   ╚═╝    ╚═════╝ ╚═╝  ╚═╝    ╚══════╝ ╚═════╝ ╚═╝     ╚═╝      ╚═════╝ ╚═╝  ╚═╝   ╚═╝
                    ── Support Tor for Freedom, Privacy ──
</pre>

# 🧅 Tor Relay Support — The Complete Freedom Guide

**Every relay you run makes the internet freer. Every byte you share defends someone's life.**

[![Tor Project](https://img.shields.io/badge/Tor_Project-Official-7D4698?style=flat-square&logo=tor-browser&logoColor=white)](https://torproject.org)
[![License](https://img.shields.io/badge/License-CC0_1.0-lightgrey?style=flat-square)](https://creativecommons.org/publicdomain/zero/1.0/)
[![Relay Guide](https://img.shields.io/badge/Setup-Middle_Relay-brightgreen?style=flat-square)](#2-vds--vps-server-setup-the-powerhouse)
[![Bridge Guide](https://img.shields.io/badge/Setup-Bridge-blue?style=flat-square)](#bridge-setup-helping-censored-users-connect)
[![Snowflake](https://img.shields.io/badge/Setup-Snowflake-cyan?style=flat-square)](#4-snowflake--the-easiest-way-to-help-no-technical-knowledge-required)
[![Raspberry Pi](https://img.shields.io/badge/Setup-Raspberry_Pi-red?style=flat-square)](#1-raspberry-pi-the-24-7-freedom-machine)
[![Free VDS List](https://img.shields.io/badge/Free_Servers-12%2B_Options-orange?style=flat-square)](#-free-vds--vps-providers-the-complete-list)
[![Donate Tor](https://img.shields.io/badge/Donate-Tor_Project-purple?style=flat-square)](https://donate.torproject.org)
[![EFF](https://img.shields.io/badge/Support-EFF-yellow?style=flat-square)](https://eff.org)
[![Network Stats](https://img.shields.io/badge/Network_Stats-Metrics.torproject.org-informational?style=flat-square)](https://metrics.torproject.org)
[![Relay Search](https://img.shields.io/badge/Find_Relays-relay.torproject.org-9cf?style=flat-square)](https://relay.torproject.org)

</div>

---

---

## Reference Videos 

<table>
  <tr>
    <td align="center">
      <a href="https://www.youtube.com/watch?v=2CJGIEunAQ0">
        <img src="https://img.youtube.com/vi/2CJGIEunAQ0/0.jpg" alt="Defend Your Privacy! How To Create Your Own Tor Relay!" width="300">
        <br>
        <strong>🇬🇧 English Guide 1</strong>
      </a>
    </td>
    <td align="center">
      <a href="https://www.youtube.com/watch?v=b7i-832Ffsw&t=364s">
        <img src="https://img.youtube.com/vi/b7i-832Ffsw/0.jpg" alt="Eski Bilgisayarınız İnterneti Özgürleştirebilir" width="300">
        <br>
        <strong>🇹🇷 Turkish Guide</strong>
      </a>
    </td>
    <td align="center">
      <a href="https://www.youtube.com/watch?v=eeFelgM70Ow">
        <img src="https://img.youtube.com/vi/eeFelgM70Ow/0.jpg" alt="How to Set Up a Tor Relay in 15 Minutes" width="300">
        <br>
        <strong>🇬🇧 English Guide 2</strong>
      </a>
    </td>
  </tr>
</table>

## 📖 Table of Contents

| # | Section | Description |
|---|---------|-------------|
| 0 | [🌍 Why This Matters](#-why-this-matters--the-case-for-internet-freedom) | What Tor is, why freedom needs it, who depends on it |
| 1 | [🧅 How Tor Works](#-how-tor-works-technically) | Onion routing, relay types explained simply |
| 2 | [⚖️ Legal & Safety](#%EF%B8%8F-legal--safety-information) | What you are and aren't responsible for |
| 3 | [🖥️ Raspberry Pi Setup](#1-raspberry-pi-the-247-freedom-machine) | Full Pi relay/bridge guide, all models |
| 4 | [☁️ VDS / VPS Setup](#vds--vps-server-setup) | Ubuntu/Debian, hardening, monitoring |
| 5 | [🆓 Free VDS Providers](#-free-vds--vps-providers-the-complete-list) | 12+ free/trial cloud servers listed |
| 6 | [🌉 Bridge Setup](#bridge-setup-helping-censored-users-connect) | obfs4, Snowflake bridge, HTTPS pluggable transport |
| 7 | [❄️ Snowflake](#4-snowflake--the-easiest-way-to-help-no-technical-knowledge-required) | Browser extension & standalone daemon |
| 8 | [💻 Personal Computer](#3-personal-computer-setup) | Running relay/bridge on Windows, Linux, macOS |
| 9 | [📊 Monitoring](#-monitoring-your-relay) | Nyx, metrics, arm, Grafana |
| 10 | [🔧 Troubleshooting](#-troubleshooting-guide) | Common problems and fixes |
| 11 | [💸 Financial Support](#-financial-support--organizations) | How to donate, who to support |
| 12 | [🔗 Resources](#-essential-links--resources) | All official links in one place |
| 13 | [⚙️ Ready-to-Use Config Files](#-ready-to-use-config-files) | Pre-configured torrc files for all setups |

---

## 🌍 Why This Matters — The Case for Internet Freedom

> *"Privacy is not something that I'm merely entitled to, it's an absolute prerequisite."* — Marlon Brando

### The Problem: The Internet Is Broken for Billions

Right now, as you read this, millions of people around the world cannot access the open internet. Not because of technical failures. Not because of slow connections. But because their governments decided they shouldn't.

- 🇨🇳 **China** blocks Google, Wikipedia, Twitter, YouTube, and tens of thousands of websites behind the "Great Firewall"
- 🇮🇷 **Iran** restricts social media, throttles VPNs, and shuts down the internet during protests
- 🇷🇺 **Russia** has blocked thousands of websites including independent news, VPNs, and parts of Wikipedia
- 🇰🇵 **North Korea** allows almost no internet access for regular citizens at all
- 🇧🇾 **Belarus**, 🇪🇹 **Ethiopia**, 🇵🇰 **Pakistan**, 🇧🇩 **Bangladesh**, and dozens of other countries apply severe internet censorship

But censorship is just one part of the problem. Even in countries with a "free" internet:

- Your **Internet Service Provider** logs every website you visit
- **Advertisers** build detailed psychological profiles of you without your consent
- **Governments** run mass surveillance programs revealed by whistleblowers like Edward Snowden
- **Corporations** monetize your behavior, fears, and desires
- **Stalkers, abusers, and criminals** can track ordinary people through their digital footprint

**Privacy is not a luxury. It is a human right.** Recognized by the UN Declaration of Human Rights (Article 12), privacy is the foundation upon which freedom of expression, assembly, and thought rest. Without privacy, there is no true freedom.

---

### The Solution: The Tor Network

Tor (The Onion Router) is a free, open-source network that provides anonymity and censorship circumvention to anyone in the world. Created by the US Naval Research Laboratory in the 1990s and later released to the public, it is now maintained by the non-profit **Tor Project**.

**Who uses Tor?**

| User Type | Why They Need Tor |
|-----------|-------------------|
| 🗞️ **Journalists** | Protect sources, access censored information, communicate securely |
| 🏥 **Human Rights Workers** | Report from conflict zones without being tracked |
| 🧑‍💻 **Activists** | Organize in countries where organizing can mean prison |
| 🔬 **Researchers** | Access information freely, without their queries being logged |
| 🔒 **Privacy-Conscious Citizens** | Simply want to browse without being surveilled |
| 🩺 **Domestic Abuse Survivors** | Escape location tracking by abusers |
| 💼 **Lawyers & Doctors** | Protect confidential client/patient communications |
| 🎓 **Students** | Access blocked academic resources |
| 🌐 **Regular People** | Because everyone deserves a private corner of the internet |

**Real examples of Tor's impact:**

- During the **2019–2022 Iranian protests** (#زن_زندگی_آزادی), over 80,000 Snowflake relays were spun up by volunteers worldwide to help Iranian citizens stay connected when the government shut down the internet
- **SecureDrop**, used by The Guardian, Washington Post, and The New York Times, runs on Tor to allow whistleblowers to safely share documents
- **Tails OS** — used by journalists and activists in war zones — routes all traffic through Tor
- Tor helps **LGBTQ+ individuals** in hostile countries access communities and resources safely

---

### Why Relays Are the Heart of It All

The Tor network doesn't run on Tor Project servers. **It runs on volunteer computers — just like yours.**

Every time someone uses Tor Browser, their traffic passes through **3 volunteer relays** before reaching the destination. This is what makes Tor anonymous:

- Relay 1 (Guard) knows who you are, but not where you're going
- Relay 2 (Middle) knows neither who you are nor where you're going
- Relay 3 (Exit) knows where you're going, but not who you are

**No single relay knows the full picture.** Each relay only encrypts what it needs to see.

When you run a relay, you become part of this chain. You become a guardian of someone's anonymity. You might be helping:

- A journalist in Belarus
- A teenager in Tehran trying to read Wikipedia
- A researcher in China accessing academic papers
- A dissident in Russia organizing a peaceful protest

You will never know who you helped. That's the point. That's beautiful.

> **The Tor network is only as strong as its volunteers. More relays = more speed, more anonymity, more resilience.** As of 2025, there are roughly 7,000–8,000 relays worldwide. The network needs more. It needs *you*.

---

## 🧅 How Tor Works (Technically)

### Onion Routing Explained Simply

Imagine you want to send a letter without anyone knowing you sent it or what's inside:

1. You put your letter in **3 envelopes**, each locked with a different padlock
2. Only Relay 3 has the key to the outermost lock
3. Only Relay 2 has the key to the second lock
4. Only Relay 1 has the key to the innermost lock
5. The final destination just gets your letter — with no return address

This is onion routing. Each layer is "peeled" by one relay, which then passes it along. No single relay can read the message AND know who sent it.

### Types of Tor Nodes

```
┌─────────────────────────────────────────────────────────────────────────┐
│                         TOR NETWORK TOPOLOGY                            │
│                                                                         │
│   [YOU]──►[Guard/Entry Relay]──►[Middle Relay]──►[Exit Relay]──►[Web]   │
│                    ↑                   ↑                  ↑             │
│              Knows your IP       Most anonymous      Knows destination  │
│              Not destination     Knows nothing       Not your IP        │
│                                                                         │
│   ┌──────────────┬────────────────────────────────────────────────┐     │
│   │ Relay Type   │ Description                                    │     │
│   ├──────────────┼────────────────────────────────────────────────┤     │
│   │ Guard/Entry  │ First hop. Users connect to this first.        │     │
│   │ Middle       │ ✅ SAFEST FOR VOLUNTEERS. Middle of the chain. │     │
│   │ Exit         │ ⚠️  Last hop. Traffic appears to come from you.│     │
│   │ Bridge       │ Unlisted relay. Helps censored users connect.  │     │
│   │ Snowflake    │ Temporary WebRTC bridge. Zero config.          │     │
│   └──────────────┴────────────────────────────────────────────────┘     │
└─────────────────────────────────────────────────────────────────────────┘
```

> ⚠️ **This guide does NOT cover Exit Node setup.** We only cover Middle Relays and Bridges, which are safe for home users and free VPS providers. Middle relays pass only encrypted traffic that cannot be read by the relay operator.

### Bandwidth and the Network

The Tor network moves roughly **250–350 Gbps** of traffic on a good day. But it needs more. Every relay you add:

- Reduces bottlenecks
- Improves speed for all users
- Makes the network harder to attack or block
- Adds geographical diversity

---

## ⚖️ Legal & Safety Information

> *This is general information, not legal advice. Laws vary by jurisdiction.*

### Middle Relays Are Safe

As a **Middle Relay** operator, you are **not** an endpoint of traffic. Your relay passes encrypted data that:

- You **cannot** read (it is encrypted with keys you don't have)
- Does **not** originate from you
- Does **not** appear to come from your IP to destination websites (that's the exit node's IP)

You are essentially a **trusted courier who carries sealed envelopes without opening them.**

Multiple legal precedents and guidance exist:

- The **Electronic Frontier Foundation (EFF)** has published legal guidance for relay operators in the USA
- The **Chaos Computer Club (CCC)** in Germany has confirmed that running non-exit Tor relays is legal
- The **Tor Project's legal FAQ** covers operator rights in many countries

### Key Rules for Safe Operation

| ✅ DO | ❌ DON'T |
|--------|----------|
| Run a Middle Relay | Run an Exit Node on home internet |
| Set `ExitRelay 0` in config | Leave ExitRelay setting unset |
| Read your VPS provider's ToS | Assume all providers allow Tor |
| Use a contact email | Ignore abuse complaints |
| Keep your system updated | Run outdated Tor software |
| Monitor your relay | Set and forget forever |

### Resource: EFF Legal Guide for Tor Operators

🔗 [https://www.eff.org/pages/legal-guide-us-tor-operators](https://www.eff.org/pages/legal-guide-us-tor-operators)

---

## 🔧 Prerequisites Checklist

Before you start any setup, verify:

```
[ ] Bandwidth: At least 10 Mbps upload AND download, ideally unlimited or high-quota
[ ] Stability: Connection is relatively stable (not mobile hotspot as primary)
[ ] Port access: You can open ports in your router/firewall (9001, 9030 by default)
[ ] OS: Linux preferred (Ubuntu 22.04+ or Debian 12+ recommended)
[ ] Awareness: You've read the legal section above
[ ] Time: Initial setup takes 30–90 minutes; ongoing maintenance is minimal
```

---

## 1. Raspberry Pi — The 24/7 Freedom Machine

A Raspberry Pi running a Tor relay is arguably one of the **most impactful privacy contributions per dollar** possible. A Pi 4 draws only **3–5 watts**, costs almost nothing to run 24/7, and can push 50–100 Mbps easily.

### Recommended Hardware

| Model | RAM | Recommended For | Notes |
|-------|-----|----------------|-------|
| Pi 3B+ | 1 GB | Light relay, bridge | Minimum; works fine |
| **Pi 4 (2GB)** | 2 GB | **Middle relay** | ✅ Best value |
| Pi 4 (4GB/8GB) | 4–8 GB | High-bandwidth relay | Overkill but great |
| Pi 5 | 4–8 GB | Maximum performance | Future-proof |
| Pi Zero 2W | 512 MB | Snowflake only | Too limited for relay |

### What You'll Need

- Raspberry Pi (3B+ or newer recommended)
- MicroSD card: **16 GB minimum**, Class 10 / A1 speed rating
- Power supply (official Pi PSU recommended — cheap ones cause instability)
- Network: **Ethernet cable strongly preferred** over Wi-Fi for stability
- (Optional) A case with cooling to prevent thermal throttling

---

### Step 0: Flash Raspberry Pi OS

Download **Raspberry Pi OS Lite** (no desktop — you don't need it):

🔗 [https://www.raspberrypi.com/software/](https://www.raspberrypi.com/software/)

Use **Raspberry Pi Imager** to flash. When configuring:

1. Enable SSH in the Imager settings
2. Set your username and password
3. Configure Wi-Fi only if you have no Ethernet option

---

### Step 1: First Boot & System Update

Connect via SSH:
```bash
ssh pi@<your-pi-ip-address>
```

Update everything:
```bash
sudo apt update && sudo apt upgrade -y
sudo apt autoremove -y
```

Set the timezone (important for logs):
```bash
sudo timedatectl set-timezone UTC
```

---

### Step 2: Install Tor from the Official Repository

The Raspberry Pi OS default Tor package can be outdated. Use the **official Tor Project repository** for the latest stable version:

```bash
# Install dependencies
sudo apt install apt-transport-https curl gpg -y

# Add Tor Project GPG key
curl -fsSL https://deb.torproject.org/torproject.org/A3C4F0F979CAA22CDBA8F512EE8CBC9E886DDD89.asc \
  | gpg --dearmor \
  | sudo tee /usr/share/keyrings/tor-archive-keyring.gpg > /dev/null

# Add Tor Project repository
# For Raspberry Pi OS (Debian-based), use the Debian codename
CODENAME=$(lsb_release -cs)
echo "deb [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] \
  https://deb.torproject.org/torproject.org $CODENAME main" \
  | sudo tee /etc/apt/sources.list.d/tor.list

# Update and install
sudo apt update
sudo apt install tor deb.torproject.org-keyring -y
```

Verify installation:
```bash
tor --version
# Should show: Tor version 0.4.x.x or newer
```

---

### Step 3: Configure Your Relay

Open the Tor configuration file:

```bash
sudo nano /etc/tor/torrc
```

**Erase the existing content** and replace with this template. Read every comment — they explain each option:

```torrc
## ============================================================
## TOR MIDDLE RELAY CONFIGURATION
## Raspberry Pi / Home Server Edition
## ============================================================

## Your relay's nickname (letters and numbers only, max 19 chars)
## This is how your relay will appear on metrics.torproject.org
Nickname MyPiRelay

## The port Tor uses for relay traffic (incoming connections from other relays/clients)
## Default: 9001. Make sure this port is open in your router (port forwarding).
ORPort 9001

## Directory port (used by clients to download network consensus)
## Set to 0 to disable if your ISP blocks it
DirPort 9030

## CRITICAL: This MUST be 0 for a middle relay (no exit traffic)
ExitRelay 0

## Reject all exit traffic (belt AND suspenders — both are good practice)
ExitPolicy reject *:*

## Disable SOCKS proxy (we're a relay, not a proxy)
SocksPort 0

## Your contact information (optional but HIGHLY recommended)
## Helps the Tor Project and abuse teams contact you
## Use a ProtonMail or similar privacy-respecting email
ContactInfo YourName <your@email.com>

## Bandwidth rate: Maximum sustained bandwidth your relay uses
## Examples: 1 MB = ~8 Mbps, 5 MB = ~40 Mbps, 10 MB = ~80 Mbps
## Start conservative and increase once relay is stable
BandwidthRate 2 MB

## Burst: Temporary peak allowed above the rate
## Set 1.5–2x your BandwidthRate
BandwidthBurst 4 MB

## If you have a monthly data limit, use AccountingMax to cap usage
## This example allows 100 GB per month (50 in + 50 out)
## Comment out if you have unlimited bandwidth
# AccountingMax 100 GB
# AccountingStart month 1 00:00

## Log level and destination
## 'notice' is the right level for normal operation
Log notice file /var/log/tor/notices.log

## Data directory for Tor's state files (keys, etc.)
DataDirectory /var/lib/tor
```

Save and exit: `Ctrl+X`, then `Y`, then `Enter`

---

### Step 4: Open Router Port

You **must** forward port **9001** (and optionally 9030) on your home router to your Pi's local IP address.

Every router is different, but the process is:

1. Log into your router (usually `http://192.168.1.1` or `http://192.168.0.1`)
2. Find **Port Forwarding** or **Virtual Server** settings
3. Add a rule:
   - **External Port:** 9001
   - **Internal IP:** Your Pi's local IP (e.g., `192.168.1.50`)
   - **Internal Port:** 9001
   - **Protocol:** TCP

Give your Pi a **static local IP** to prevent the forwarding rule breaking:
```bash
# Note your current IP
hostname -I

# Then configure static IP in /etc/dhcpcd.conf or via your router's DHCP reservation
```

---

### Step 5: Start and Enable Tor

```bash
# Start Tor
sudo systemctl start tor

# Enable it to start on every boot
sudo systemctl enable tor

# Check status (should say "Active: active (running)")
sudo systemctl status tor

# Watch the logs (wait 2–3 minutes for bootstrapping)
sudo tail -f /var/log/tor/notices.log
```

**What to look for in logs:**

```
[notice] Bootstrapped 0% (starting): Starting
[notice] Bootstrapped 14% (handshake): Handshaking with a relay
[notice] Bootstrapped 25% (loading_status): Loading relay status
[notice] Bootstrapped 100% (done): Done
```

Once you see **Bootstrapped 100%**, your relay is live. 🎉

---

### Step 6: Verify Your Relay Is Public

After about **3 hours**, your relay will appear in the public Tor directory. Search for it:

🔗 [https://metrics.torproject.org/rs.html](https://metrics.torproject.org/rs.html) — search by your Nickname

🔗 [https://relay.torproject.org](https://relay.torproject.org) — official relay operator hub

---

### Step 7: Install Nyx (Relay Monitor)

Nyx is a terminal-based dashboard for your Tor relay — like `htop` but for Tor.

```bash
sudo apt install nyx -y
```

Run it:
```bash
sudo -u debian-tor nyx
```

```
┌─ nyx ─────────────────────────────────────────────────────────────────┐
│ Uptime: 3 days, 4:22:10  Fingerprint: A3F9...                         │
├───────────────────────────────────────────────────────────────────────┤
│ ↑ 1.87 MB/s ↓ 2.03 MB/s  Bandwidth: Rate 2.0 MB/s Burst 4.0 MB/s      │
│ Connections: 143 (Guard: 0, Middle: 143, Dir: 0)                      │
│ [████████████████████████░░░░░░░░] 71% Bandwidth Used                 │
└───────────────────────────────────────────────────────────────────────┘
```

Use arrow keys to navigate between panels. `q` to quit.

---

### Optional: Keep Your Pi Secure

```bash
# Change default password
passwd

# Disable password SSH login (use SSH keys instead)
# (Advanced — look up "SSH key authentication" if unfamiliar)

# Install automatic security updates
sudo apt install unattended-upgrades -y
sudo dpkg-reconfigure -plow unattended-upgrades

# Install fail2ban to block brute-force SSH attempts
sudo apt install fail2ban -y
sudo systemctl enable fail2ban
sudo systemctl start fail2ban
```

---

## 2. VDS / VPS Server Setup — The Powerhouse

A Virtual Dedicated Server (VDS/VPS) is a rented cloud server. For Tor, this is ideal because:

- **Always on** — no need to keep a home computer running
- **Better bandwidth** — often 1–10 Gbps port
- **No home IP exposed** — your home address is not associated with the relay
- **Global diversity** — choose server locations underrepresented in Tor's network

### Recommended OS: Ubuntu 22.04 LTS or Debian 12

Both are excellent. Ubuntu is beginner-friendlier; Debian is more minimal. All commands below work on both.

---

### Step 1: Initial Server Hardening

After logging in to your new VPS for the first time:

```bash
# Update everything
sudo apt update && sudo apt upgrade -y

# Set hostname (optional but helpful)
sudo hostnamectl set-hostname my-tor-relay

# Create a non-root user (never run Tor as root permanently)
sudo adduser toroperator
sudo usermod -aG sudo toroperator

# Switch to new user
su - toroperator
```

---

### Step 2: Configure UFW Firewall

```bash
# Install UFW if not present
sudo apt install ufw -y

# Default policies
sudo ufw default deny incoming
sudo ufw default allow outgoing

# Allow SSH (CRITICAL: do this BEFORE enabling UFW or you'll lock yourself out)
sudo ufw allow 22/tcp

# Allow Tor relay port
sudo ufw allow 9001/tcp

# Allow Tor directory port (optional)
sudo ufw allow 9030/tcp

# Enable firewall
sudo ufw enable

# Verify
sudo ufw status verbose
```

---

### Step 3: Install Tor from Official Repository

```bash
# Install dependencies
sudo apt install apt-transport-https curl gpg -y

# Add Tor Project GPG key
curl -fsSL https://deb.torproject.org/torproject.org/A3C4F0F979CAA22CDBA8F512EE8CBC9E886DDD89.asc \
  | gpg --dearmor \
  | sudo tee /usr/share/keyrings/tor-archive-keyring.gpg > /dev/null

# Detect your OS codename
CODENAME=$(lsb_release -cs)
echo "Detected codename: $CODENAME"

# Add repository
echo "deb [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] \
  https://deb.torproject.org/torproject.org $CODENAME main" \
  | sudo tee /etc/apt/sources.list.d/tor.list

# Install
sudo apt update
sudo apt install tor deb.torproject.org-keyring -y

# Verify
tor --version
```

---

### Step 4: VPS torrc Configuration

```bash
sudo nano /etc/tor/torrc
```

VPS-optimized configuration:

```torrc
## ============================================================
## TOR MIDDLE RELAY CONFIGURATION
## VPS / Cloud Server Edition
## ============================================================

## Relay identity
Nickname MyVPSRelay
ContactInfo YourName <your@email.com>

## Ports
ORPort 9001
DirPort 9030

## Safety settings — non-negotiable
ExitRelay 0
ExitPolicy reject *:*
SocksPort 0

## VPS typically has much better bandwidth than Pi
## Adjust to ~80% of your actual available bandwidth
## If you have 1 Gbps: use 100 MB (800 Mbps)
## If you have 100 Mbps: use 10 MB (80 Mbps)
BandwidthRate 10 MB
BandwidthBurst 20 MB

## For VPS with monthly traffic limits, set accounting
## Example: 500 GB/month (total in+out)
# AccountingMax 500 GB
# AccountingStart month 1 00:00

## Logging
Log notice file /var/log/tor/notices.log

## Data directory
DataDirectory /var/lib/tor

## IPv6 support (highly recommended if your VPS has an IPv6 address)
## Find your IPv6 with: ip -6 addr show
# ORPort [your::ipv6::address]:9001

## If your VPS blocks DirPort, comment it out and only use:
# DirPort 0
```

---

### Step 5: Start and Enable

```bash
sudo systemctl restart tor
sudo systemctl enable tor
sudo systemctl status tor

# Watch logs
sudo journalctl -u tor -f
# OR
sudo tail -f /var/log/tor/notices.log
```

---

### Step 6: Install Nyx for Monitoring

```bash
sudo apt install nyx -y

# Run as the Tor user
sudo -u debian-tor nyx
```

For persistent monitoring with Grafana and Prometheus, see the [Monitoring section](#-monitoring-your-relay) below.

---

### Step 7: Set Up Automatic Updates

```bash
sudo apt install unattended-upgrades -y
sudo dpkg-reconfigure -plow unattended-upgrades
```

Edit `/etc/apt/apt.conf.d/50unattended-upgrades` to also auto-update Tor:

```bash
sudo nano /etc/apt/apt.conf.d/50unattended-upgrades
```

Ensure this line is uncommented:
```
"${distro_id}:${distro_codename}-security";
```

---

## 🆓 Free VDS / VPS Providers — The Complete List

> ⚠️ **Always read the provider's Terms of Service before running Tor.** Most free/trial providers are fine with middle relays. Exit nodes should never be run on shared/free hosting.

### 🏆 Tier 1: Always Free (No Expiry)

---

#### 1. Oracle Cloud Free Tier ⭐ BEST OPTION

🔗 **Sign up:** [https://cloud.oracle.com/free](https://cloud.oracle.com/free)

Oracle offers the most generous "Always Free" cloud tier available anywhere. No expiry, no credit card required after sign-up verification.

**Free forever specs:**
- 2× AMD VM instances: 1 vCPU, 1 GB RAM each (Micro)
- **OR** up to 4 ARM Ampere A1 instances totaling 4 OCPUs and 24 GB RAM (configurable!)
- 200 GB total block storage
- **10 TB outbound bandwidth per month** 🤯
- Free object storage, databases, monitoring

**For Tor:** Use the ARM A1 instances. You can run a **4-core, 24 GB RAM** VM for free. This is more powerful than most paid VPS under $20/month.

**Oracle-specific setup — open firewall ports:**
```bash
# Oracle blocks ports via their "Security Lists" in addition to the OS firewall
# You MUST open ports in BOTH places

# 1. UFW (OS firewall) — same as above
sudo ufw allow 9001/tcp
sudo ufw allow 9030/tcp
sudo ufw enable

# 2. Go to Oracle Cloud Console:
#    Networking → Virtual Cloud Networks → Your VCN
#    → Security Lists → Default Security List
#    → Add Ingress Rule:
#      Source CIDR: 0.0.0.0/0
#      Protocol: TCP
#      Destination Port Range: 9001
#    → Save
```

> 💡 **Tip:** Oracle's ARM A1 instances in us-ashburn-1 or us-phoenix-1 often have inventory. If you get "out of capacity" errors, try again at different times of day.

---

#### 2. Google Cloud Free Tier

🔗 **Sign up:** [https://cloud.google.com/free](https://cloud.google.com/free)

**Always free (after trial):**
- 1× e2-micro VM in select US regions (us-west1, us-central1, us-east1)
- 30 GB HDD storage
- 1 GB network egress per month to most regions

**Trial:**
- $300 credit for 90 days (enough to run a more powerful relay for 3 months)

**Tor suitability:** The free e2-micro (0.25–2 vCPU, 1 GB RAM) is modest but sufficient for a basic middle relay. Keep `BandwidthRate` at 1–2 MB to avoid egress charges.

**Google Cloud setup:**
```bash
# After creating your VM, open firewall in Console:
# VPC Network → Firewall → Create Firewall Rule
# Name: allow-tor-relay
# Direction: Ingress
# Targets: All instances
# Source IP ranges: 0.0.0.0/0
# Protocols: TCP port 9001, 9030
```

---

#### 3. IBM Cloud Free Tier

🔗 [https://cloud.ibm.com/registration](https://cloud.ibm.com/registration)

- Free Lite account with limited compute
- Kubernetes free tier (more complex to use)
- Good for experienced Linux users
- 256 MB RAM on free containers (very limited for relay)

**Best use:** Running a Snowflake standalone daemon rather than a full relay.

---

### 🥈 Tier 2: Trial Credits (12 Months or Large Credits)

---

#### 4. Amazon Web Services (AWS) Free Tier

🔗 [https://aws.amazon.com/free/](https://aws.amazon.com/free/)

**12-month free:**
- 750 hours/month of t2.micro or t3.micro (1 vCPU, 1 GB RAM)
- That's effectively one instance running 24/7 for a year, free

**Setup:**
```bash
# AWS uses Security Groups for firewall
# In AWS Console: EC2 → Security Groups → Your group
# Add Inbound Rule:
# Type: Custom TCP, Port: 9001, Source: 0.0.0.0/0
# Type: Custom TCP, Port: 9030, Source: 0.0.0.0/0
```

> ⚠️ **Set up billing alerts!** AWS will charge you after 12 months. Go to Billing → Budgets and set a $1 threshold alert.

---

#### 5. Microsoft Azure Free Tier

🔗 [https://azure.microsoft.com/free/](https://azure.microsoft.com/free/)

**Trial:**
- $200 credit for 30 days
- 12 months of free B1S Linux VM (1 vCPU, 1 GB RAM)

**Setup NSG (Network Security Group):**
```bash
# In Azure Portal:
# VM → Networking → Add Inbound Port Rule
# Protocol: TCP, Port: 9001, Action: Allow
```

---

#### 6. DigitalOcean

🔗 [https://www.digitalocean.com/try/free-trial](https://www.digitalocean.com/try/free-trial)

- $200 credit for 60 days for new accounts
- Simple UI — arguably the most beginner-friendly VPS experience
- Droplets start at $4/month for 512 MB RAM

**DigitalOcean firewall setup:**
```bash
# Networking → Firewalls → Create Firewall
# Add Inbound Rule: TCP 9001 from All IPv4 and All IPv6
# Apply to your Droplet
```

---

#### 7. Vultr

🔗 [https://www.vultr.com/promo/try50/](https://www.vultr.com/promo/try50/)

- $50–$100 trial credits (check current promo)
- Fast NVMe storage
- 25+ global locations
- Very simple API and CLI

---

#### 8. Linode / Akamai Cloud

🔗 [https://linode.com](https://linode.com)

- $100 credit for 60 days for new accounts
- Excellent documentation
- Strong Linux community support

---

#### 9. Hetzner Cloud (Europe)

🔗 [https://www.hetzner.com/cloud/](https://www.hetzner.com/cloud/)

- Not free, but **extremely cheap**: €3.79/month for CX22 (2 vCPU, 4 GB RAM, 20 TB traffic)
- Based in Germany and Finland — **excellent for Tor network diversity**
- Tor is explicitly permitted in their ToS for middle relays
- Among the most popular VPS providers for Tor operators in Europe

---

#### 10. Contabo

🔗 [https://contabo.com](https://contabo.com)

- Very affordable German provider: ~€5/month for 4 vCPU, 8 GB RAM, 32 TB traffic
- Large bandwidth allocation makes it excellent for high-bandwidth relays
- No free tier, but extremely good value

---

#### 11. Fly.io

🔗 [https://fly.io](https://fly.io)

- Generous free tier for small apps/containers
- More complex Docker-based deployment
- Distributed infrastructure across many regions
- Good for advanced users wanting to deploy Tor in containers

---

#### 12. Railway

🔗 [https://railway.app](https://railway.app)

- $5 free credit per month with GitHub login
- Container-based, good for Snowflake daemon
- Quick deploy environment

---

### 📋 Quick Comparison Table

| Provider | Free Tier | RAM | Bandwidth | Best For | ToS Friendly |
|----------|-----------|-----|-----------|----------|--------------|
| Oracle Cloud | ✅ Always Free | Up to 24 GB | 10 TB/mo | **Full relay** | ✅ |
| Google Cloud | ✅ Always Free + $300 | 1 GB | 1 GB free | Light relay | ✅ |
| AWS | ✅ 12 months | 1 GB | Pay per GB | Relay | ✅ |
| Azure | $200/30d, 12mo free | 1 GB | Pay per GB | Relay | ✅ |
| DigitalOcean | $200/60d | 512 MB–2 GB | 500 GB/mo | Relay | ✅ |
| Vultr | $50–100 credits | 1 GB+ | 1 TB/mo | Relay | Check |
| Linode | $100/60d | 1 GB+ | 1 TB/mo | Relay | ✅ |
| Hetzner | ❌ (€3.79/mo) | 4 GB | 20 TB/mo | **High-BW relay** | ✅ |
| Contabo | ❌ (~€5/mo) | 8 GB | 32 TB/mo | **Power relay** | ✅ |
| IBM Cloud | ✅ Always Free | 256 MB | Limited | Snowflake only | Check |

---

## Bridge Setup: Helping Censored Users Connect

Bridges are **unlisted Tor relays** — they don't appear in the public Tor directory, making them much harder for censors to block. When Iran, Russia, or China block all known Tor relays, users fall back to bridges.

### Why Bridges Matter

```
Normal Tor user:
  [User] → connects to public relay list → [Guard Relay] → ...

Censored country user:
  [User in Iran] → public relays ALL BLOCKED → gets bridge address from
                   bridges.torproject.org or a friend → [Bridge] → ...
```

Bridges with **Pluggable Transports** disguise Tor traffic to look like normal HTTPS or video streaming traffic, making deep-packet inspection (DPI) much harder to use for blocking.

### Types of Pluggable Transports

| Transport | What It Does | Best For |
|-----------|-------------|----------|
| `obfs4` | Obfuscates traffic shape | Most countries |
| `webtunnel` | Wraps traffic as HTTPS | China, Iran |
| `meek-azure` | Routes through Microsoft Azure CDN | Extreme censorship |
| `Snowflake` | WebRTC — looks like video calls | China, Russia |

---

### Bridge Setup (obfs4 — Most Common)

```bash
# Install Tor and pluggable transports
sudo apt install tor obfs4proxy -y
```

```bash
sudo nano /etc/tor/torrc
```

```torrc
## ============================================================
## TOR BRIDGE CONFIGURATION WITH OBFS4
## ============================================================

## Tell Tor this is a bridge
BridgeRelay 1

## Port for Tor traffic (bridge uses a single ORPort)
## You can use 443 or 80 to look like HTTPS/HTTP traffic
ORPort 443

## ServerTransportPlugin for obfs4
## This makes your bridge use the obfs4 obfuscation layer
ServerTransportPlugin obfs4 exec /usr/bin/obfs4proxy

## Port that obfs4 listens on (what censored users actually connect to)
ServerTransportListenAddr obfs4 0.0.0.0:9002

## Don't publish to the main directory (that's the point of a bridge!)
PublishServerDescriptor 0

## Safety settings
ExitRelay 0
ExitPolicy reject *:*
SocksPort 0

## Contact and nickname
ContactInfo your@email.com
Nickname MyBridge

## Rate limiting (bridges often used by people with metered connections)
BandwidthRate 5 MB
BandwidthBurst 10 MB

Log notice file /var/log/tor/notices.log
DataDirectory /var/lib/tor
```

Start and enable:
```bash
sudo systemctl restart tor
sudo systemctl enable tor
```

Find your bridge line to share:
```bash
sudo cat /var/lib/tor/pt_state/obfs4_bridgeline.txt
```

This outputs something like:
```
Bridge obfs4 1.2.3.4:9002 FINGERPRINT cert=XXXXX iat-mode=0
```

Share this line with people who need it via Signal, PGP-encrypted email, or [bridges.torproject.org](https://bridges.torproject.org) if you register it.

---

### WebTunnel Bridge Setup (For China/Iran)

WebTunnel makes your bridge look like a legitimate HTTPS website — much harder to block with DPI.

```bash
# Download webtunnel binary
wget https://github.com/net4people/bbs/raw/master/webtunnel -O /usr/local/bin/webtunnel
chmod +x /usr/local/bin/webtunnel
```

```torrc
BridgeRelay 1
ORPort 443
ServerTransportPlugin webtunnel exec /usr/local/bin/webtunnel
ServerTransportListenAddr webtunnel 0.0.0.0:443
ExitRelay 0
ExitPolicy reject *:*
SocksPort 0
ContactInfo your@email.com
Nickname MyWebTunnel
```

🔗 Full WebTunnel guide: [https://community.torproject.org/relay/setup/webtunnel/](https://community.torproject.org/relay/setup/webtunnel/)

---

## 4. Snowflake — The Easiest Way to Help (No Technical Knowledge Required)

Snowflake is **zero-configuration** support for Tor. You share a tiny amount of bandwidth, and users in censored countries use your connection as a WebRTC proxy to reach the Tor network.

You don't need to open ports. You don't need a server. Your IP barely matters. You don't need to install anything complex.

```
Censored User
    ↓
[Snowflake Broker] ← finds available Snowflakes
    ↓
[Your Browser / Computer — Snowflake Proxy]
    ↓
[Tor Bridge] → Tor Network → Internet
```

### Method A: Browser Extension (Easiest — 2 Clicks)

**Firefox:**
🔗 [https://addons.mozilla.org/firefox/addon/torproject-snowflake/](https://addons.mozilla.org/firefox/addon/torproject-snowflake/)

**Chrome / Chromium / Edge:**
🔗 [https://chromewebstore.google.com/detail/snowflake/mafpmfcccpbjnhfhjnllmmalhifmlcie](https://chromewebstore.google.com/detail/snowflake/mafpmfcccpbjnhfhjnllmmalhifmlcie)

After installing:
1. Click the Snowflake icon in your toolbar
2. Toggle it **ON**
3. That's it. Your browser now helps censored users connect to Tor.

It uses virtually no CPU. Bandwidth usage is typically **under 50 MB/day**. You can leave it running indefinitely.

---

### Method B: Web Page (No Install Required)

Just open this page in a browser tab and leave it open:

🔗 [https://snowflake.torproject.org/embed](https://snowflake.torproject.org/embed)

---

### Method C: Standalone Snowflake Proxy (Linux/macOS — Terminal)

For maximum performance, run the Snowflake daemon directly. No browser needed.

**Install Go first (if not installed):**
```bash
sudo apt install golang-go -y
```

**Install Snowflake proxy:**
```bash
go install gitlab.torproject.org/tpo/anti-censorship/pluggable-transports/snowflake/v2/proxy@latest
```

**Run it:**
```bash
~/go/bin/proxy
```

**Run it persistently with systemd:**

```bash
sudo nano /etc/systemd/system/snowflake-proxy.service
```

```ini
[Unit]
Description=Tor Snowflake Proxy
After=network.target

[Service]
User=nobody
ExecStart=/home/YOUR_USERNAME/go/bin/proxy
Restart=on-failure
RestartSec=5

[Install]
WantedBy=multi-user.target
```

```bash
sudo systemctl daemon-reload
sudo systemctl enable snowflake-proxy
sudo systemctl start snowflake-proxy
sudo systemctl status snowflake-proxy
```

---

### Method D: Docker Snowflake

```bash
docker run -d \
  --name snowflake \
  --restart unless-stopped \
  registry.gitlab.com/tpo/anti-censorship/pluggable-transports/snowflake/v2/proxy:latest
```

---

## 3. Personal Computer Setup

You can run a relay directly on your Linux, macOS, or Windows machine — great for when you want to contribute while your computer is on without buying hardware.

### Linux (Ubuntu/Debian Desktop)

Same as the VPS setup above. The main differences:

- Use `BandwidthRate 1 MB` or less to avoid saturating your home connection
- Consider adding an **accounting rule** to avoid monthly data caps:

```torrc
## Cap at 50 GB/month total
AccountingMax 50 GB
AccountingStart month 1 00:00
```

- Create a simple startup script so the relay only runs when you're home:

```bash
# Add to your user's autostart or cron
sudo systemctl start tor  # When you want it running
sudo systemctl stop tor   # When you're done
```

### macOS

```bash
# Install Homebrew if you don't have it
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Tor
brew install tor

# Find the config file location
brew info tor
# Usually: /opt/homebrew/etc/tor/torrc or /usr/local/etc/tor/torrc

# Edit config
nano $(brew --prefix)/etc/tor/torrc

# Add same config as Linux setup above

# Start
brew services start tor

# Stop
brew services stop tor
```

### Windows

> ⚠️ Windows is **not recommended** for running a 24/7 relay. Use it for Snowflake (browser extension) or as a temporary relay when you can't use Linux.

1. Download the **Tor Expert Bundle** from:
   🔗 [https://www.torproject.org/download/tor/](https://www.torproject.org/download/tor/)

2. Extract to `C:\tor\`

3. Create `C:\tor\torrc`:
```
Nickname MyWindowsRelay
ORPort 9001
ExitRelay 0
ExitPolicy reject *:*
SocksPort 0
BandwidthRate 1 MB
BandwidthBurst 2 MB
ContactInfo your@email.com
DataDirectory C:\tor\data
Log notice file C:\tor\tor.log
```

4. Open **Windows Firewall** and allow TCP port 9001 inbound

5. Run Tor from Command Prompt:
```cmd
cd C:\tor
tor.exe -f torrc
```

6. To run as a Windows Service:
```cmd
tor.exe --service install -options -f "C:\tor\torrc"
tor.exe --service start
```

---

## 📊 Monitoring Your Relay

### Nyx — Terminal Dashboard

```bash
sudo apt install nyx -y
sudo -u debian-tor nyx
```

| Nyx Screen | What It Shows |
|------------|---------------|
| `1` | Real-time bandwidth graph |
| `2` | Active connections |
| `3` | Tor configuration |
| `4` | Log messages |

---

### metrics.torproject.org — Your Relay's Public Profile

Once your relay has been running for a few hours, find its public profile:

🔗 [https://metrics.torproject.org/rs.html#search/YourNickname](https://metrics.torproject.org/rs.html)

This shows:
- Your relay's fingerprint
- Observed bandwidth
- Consensus weight (how much traffic is routed through you)
- Uptime history
- Flags assigned (Running, Valid, Guard, HSDir, etc.)

**Relay flags:**

| Flag | Meaning | How to Get It |
|------|---------|--------------|
| `Running` | Relay is online | Automatic |
| `Valid` | In good standing | Automatic |
| `Guard` | Can be used as first hop | 8+ days uptime, stable bandwidth |
| `Stable` | Long uptime history | 8+ days |
| `Fast` | High bandwidth | High measured bandwidth |
| `HSDir` | Helps hidden services | Stable + DirPort open |

---

### Grafana + Prometheus (Advanced Monitoring)

For serious operators who want dashboards:

```bash
# Install Prometheus node exporter
sudo apt install prometheus-node-exporter -y

# Install and configure Grafana
wget -q -O - https://packages.grafana.com/gpg.key | sudo apt-key add -
echo "deb https://packages.grafana.com/oss/deb stable main" | \
  sudo tee /etc/apt/sources.list.d/grafana.list
sudo apt update && sudo apt install grafana -y
sudo systemctl enable grafana-server
sudo systemctl start grafana-server
```

🔗 Tor Relay Grafana Dashboard: [https://grafana.com/grafana/dashboards/13550](https://grafana.com/grafana/dashboards/13550)

---

## 🔧 Troubleshooting Guide

### Problem: Tor doesn't start / exits immediately

```bash
# Check the log
sudo journalctl -u tor --no-pager -n 50

# Common causes:
# - Config file syntax error
# - Port already in use
# - Permission issue on DataDirectory
```

Check your config for syntax errors:
```bash
sudo -u debian-tor tor --verify-config
```

### Problem: Stuck at "Bootstrapped X%"

```bash
# Check if port 9001 is reachable from outside
# From another machine or use an online port checker:
# https://www.portchecker.co/

# Locally check if Tor is listening:
sudo ss -tlnp | grep 9001
```

If the port isn't open:
```bash
# Check UFW
sudo ufw status

# Check if router port forwarding is set (home setup)
# Or cloud security group / firewall rules (VPS setup)
```

### Problem: Relay not appearing in metrics after 24 hours

```bash
# Verify DirPort is accessible
curl -s https://check.torproject.org/cgi-bin/TorBulkExitList.py

# Check your relay's fingerprint
sudo cat /var/lib/tor/fingerprint

# Search for it
# https://metrics.torproject.org/rs.html#search/<fingerprint>
```

### Problem: High memory usage on Pi

```bash
# Check RAM usage
free -h

# Tor should use < 100 MB normally
# If much higher, reduce MaxMemInQueues in torrc:
echo "MaxMemInQueues 256 MB" | sudo tee -a /etc/tor/torrc
sudo systemctl restart tor
```

### Problem: Bandwidth is much lower than expected

```bash
# Verify your actual available bandwidth first
curl -s https://raw.githubusercontent.com/sivel/speedtest-cli/master/speedtest.py | python3 -

# New relays get very little traffic for the first 2-3 weeks (ramp-up period)
# This is normal! The Tor directory authorities slowly increase your consensus weight.
# Be patient.
```

### Checking Your Public IP (for relay config)

```bash
curl -4 ifconfig.me  # IPv4
curl -6 ifconfig.me  # IPv6
```

---

## 💸 Financial Support & Organizations

Running a relay isn't the only way to support internet freedom. Financial donations directly fund development of Tor Browser, Tails OS, Snowflake, new pluggable transports, and the researchers who keep the network safe.

### 🧅 The Tor Project (Primary)

The Tor Project is a 501(c)(3) nonprofit. Donations are tax-deductible in the United States.

🔗 **Donate:** [https://donate.torproject.org](https://donate.torproject.org)
🔗 **European donors (EUR):** [https://opencollective.com/thetorproject-europe](https://opencollective.com/thetorproject-europe)

Accepts: Credit card, PayPal, Bitcoin, Zcash, Monero, wire transfer

The Tor Project uses donations to:
- Pay developers maintaining Tor Browser, Tor daemon, Snowflake
- Fund security audits and academic research
- Support the Tails OS project
- Maintain the Tor network infrastructure and directory authorities

---

### 🛡️ Electronic Frontier Foundation (EFF)

The EFF is the leading digital rights nonprofit in the world. They provided the original funding to create the Tor Project in 2004, publish the EFF Atlas of Surveillance, fight government overreach in court, and publish Surveillance Self-Defense guides.

🔗 **Donate:** [https://eff.org/donate](https://eff.org/donate)
🔗 **Surveillance Self-Defense:** [https://ssd.eff.org](https://ssd.eff.org)

---

### 🗞️ Freedom of the Press Foundation

Maintains **SecureDrop** — the whistleblower submission system used by The Guardian, Washington Post, NYT, and 100+ other newsrooms. It runs entirely over Tor.

🔗 **Donate:** [https://freedom.press/donate/](https://freedom.press/donate/)
🔗 **SecureDrop:** [https://securedrop.org](https://securedrop.org)

---

### 🔏 Access Now

A nonprofit defending and extending digital rights globally. Runs a Digital Security Helpline for journalists and activists in crisis.

🔗 [https://accessnow.org/donate/](https://accessnow.org/donate/)

---

### 🌐 Article 19

Works on freedom of expression and freedom of information globally, including digital rights.

🔗 [https://www.article19.org/donate/](https://www.article19.org/donate/)

---

### 🏠 Riseup

Provides secure email, VPN, and hosting for activists and nonprofits. Long-time supporter of Tor and privacy infrastructure.

🔗 [https://riseup.net/donate](https://riseup.net/donate)

---

### 🔐 Let's Encrypt / ISRG

Provides free TLS/SSL certificates, making HTTPS ubiquitous. Foundational to web privacy.

🔗 [https://letsencrypt.org/donate/](https://letsencrypt.org/donate/)

---

### 🐧 Tails OS

A live operating system you boot from USB that routes **all** traffic through Tor automatically. Used by journalists, activists, and whistleblowers worldwide.

🔗 [https://tails.net/donate/](https://tails.net/donate/)

---

### 📋 Summary Donation Table

| Organization | Focus | Link |
|-------------|-------|------|
| 🧅 Tor Project | Anonymity network & browser | [donate.torproject.org](https://donate.torproject.org) |
| 🛡️ EFF | Digital rights & legal defense | [eff.org/donate](https://eff.org/donate) |
| 🗞️ Freedom of the Press Foundation | Secure journalism | [freedom.press/donate](https://freedom.press/donate/) |
| 🔏 Access Now | Digital rights helpline | [accessnow.org/donate](https://accessnow.org/donate/) |
| 🏠 Riseup | Secure activist infrastructure | [riseup.net/donate](https://riseup.net/donate) |
| 🔒 Tails OS | Anonymous live OS | [tails.net/donate](https://tails.net/donate/) |
| 🌐 Let's Encrypt | Free HTTPS certificates | [letsencrypt.org/donate](https://letsencrypt.org/donate/) |

---

## 🔗 Essential Links & Resources

### Official Tor Resources

| Resource | URL |
|----------|-----|
| Tor Project Main Site | [https://torproject.org](https://torproject.org) |
| Tor Browser Download | [https://www.torproject.org/download/](https://www.torproject.org/download/) |
| Relay Operator Guide | [https://community.torproject.org/relay/](https://community.torproject.org/relay/) |
| Relay Setup (Official) | [https://community.torproject.org/relay/setup/](https://community.torproject.org/relay/setup/) |
| Relay Search / Metrics | [https://metrics.torproject.org/rs.html](https://metrics.torproject.org/rs.html) |
| Network Statistics | [https://metrics.torproject.org](https://metrics.torproject.org) |
| Bridge Request | [https://bridges.torproject.org](https://bridges.torproject.org) |
| Relay Operator Hub | [https://relay.torproject.org](https://relay.torproject.org) |
| Official Tor Blog | [https://blog.torproject.org](https://blog.torproject.org) |
| Tor Support / FAQ | [https://support.torproject.org](https://support.torproject.org) |
| Legal FAQ for Operators | [https://community.torproject.org/relay/community-resources/eff-tor-legal-faq/](https://community.torproject.org/relay/community-resources/eff-tor-legal-faq/) |

### Community & Discussion

| Resource | URL |
|----------|-----|
| Tor Forum | [https://forum.torproject.org](https://forum.torproject.org) |
| Tor on GitLab | [https://gitlab.torproject.org](https://gitlab.torproject.org) |
| Tor Relay Operators Mailing List | [https://lists.torproject.org/cgi-bin/mailman/listinfo/tor-relays](https://lists.torproject.org/cgi-bin/mailman/listinfo/tor-relays) |
| r/TOR on Reddit | [https://reddit.com/r/TOR](https://reddit.com/r/TOR) |

### Privacy & Security Guides

| Resource | URL |
|----------|-----|
| EFF Surveillance Self-Defense | [https://ssd.eff.org](https://ssd.eff.org) |
| Security in a Box | [https://securityinabox.org](https://securityinabox.org) |
| Privacy Guides | [https://privacyguides.org](https://privacyguides.org) |
| Tails OS | [https://tails.net](https://tails.net) |

### Tools & Monitoring

| Resource | URL |
|----------|-----|
| Nyx (Relay Monitor) | [https://nyx.torproject.org](https://nyx.torproject.org) |
| Tor Atlas (Relay Viewer) | [https://metrics.torproject.org/rs.html](https://metrics.torproject.org/rs.html) |
| OrNetStats | [https://nusenu.github.io/OrNetStats/](https://nusenu.github.io/OrNetStats/) |
| Tor Weather (Uptime Alerts) | [https://weather.torproject.org](https://weather.torproject.org) |

---

## ❓ Frequently Asked Questions

**Q: Will running a relay get me in trouble with my ISP?**
A: Middle relays pass only encrypted data that your ISP cannot read. Most ISPs have no issue with this. You can always ask your ISP's policy, or check their ToS. Avoid running an Exit Node.

**Q: How much bandwidth will a relay use?**
A: Exactly what you configure in `BandwidthRate`. Set it to 1 MB = ~8 Mbps max. A relay configured at 1 MB rate running 24/7 uses about 250 GB/month.

**Q: My relay has been running for 3 days but gets almost no traffic. Is something broken?**
A: No — this is normal. New relays have a "ramp-up" period lasting 1–3 weeks as the Tor network slowly increases your relay's consensus weight. Be patient.

**Q: Can I run multiple relays?**
A: Yes! If you run 2+ relays from the same network, set `MyFamily` in each relay's config with the fingerprints of your other relays. This prevents them from being in the same circuit.

**Q: What is a Guard relay?**
A: After ~8 days of stable uptime and good bandwidth, your relay may receive the `Guard` flag. This means Tor clients can use your relay as their first hop — a position of greater responsibility (and higher traffic).

**Q: Can I run a relay on Windows Subsystem for Linux (WSL)?**
A: Technically yes, but WSL doesn't easily expose TCP ports to the internet, making relay operation difficult. Use a real Linux install or a VM instead.

**Q: Will this slow down my internet?**
A: Only by whatever `BandwidthRate` you set. Set it below your total bandwidth and you'll never notice it.

**Q: What happens if I need to shut down temporarily?**
A: Just stop the service: `sudo systemctl stop tor`. Your relay's uptime history in the Tor directory is maintained and will recover once you restart.

---

## 🌱 The Bigger Picture

You've read this far. That means you understand something many people don't:

**The internet is infrastructure, and infrastructure needs caretakers.**

Roads need maintenance. Libraries need volunteers. The postal system needs workers. The free internet needs relay operators.

Every time a journalist safely contacts a source, every time a teenager in Iran reads a Wikipedia article about history, every time a domestic abuse survivor looks up resources without being tracked — that happens because someone, somewhere, ran a relay. Gave a few megabits per second. Shared their bandwidth.

That someone can be you.

You don't need to be a hacker. You don't need to be technical. You need a computer, an internet connection, and five minutes.

**The onion network is only as strong as the people who believe in it.**

🧅 **Run a relay. Be the network. Defend the free internet.**

---

<div align="center">

*This guide is released under CC0 — no rights reserved. Copy it, share it, translate it, improve it.*

*Pull requests welcome. Issues welcome. All contributions to freedom are welcome.*

**🧅 tor | 🛡️ eff | ❄️ snowflake | 🗞️ press freedom | 🔒 privacy | ✊ human rights**

[![Tor Project](https://img.shields.io/badge/Powered_by-Tor_Network-7D4698?style=for-the-badge&logo=tor-browser&logoColor=white)](https://torproject.org)
[![EFF Member](https://img.shields.io/badge/Support-EFF-yellow?style=for-the-badge)](https://eff.org/donate)
[![CC0](https://img.shields.io/badge/License-CC0_1.0-lightgrey?style=for-the-badge)](https://creativecommons.org/publicdomain/zero/1.0/)

</div>

## ⚙️ Ready-to-Use Config Files

You can find pre-configured `torrc` files for each setup in the [`configs/`](configs/) directory:

- [Raspberry Pi](configs/raspberry-pi/torrc)
- [VPS / Cloud Server](configs/vps/torrc)
- [Bridge with obfs4](configs/bridge/torrc-obfs4)
- [Personal Computer (Linux)](configs/personal-computer/torrc-linux)
- [Personal Computer (macOS)](configs/personal-computer/torrc-macos)
- [Personal Computer (Windows)](configs/personal-computer/torrc-windows)
- [Snowflake Systemd Service](configs/snowflake/snowflake-proxy.service)

### Thanks to [Claude AI](https://github.com/claude) for the coloring, alignment, and formatting.
