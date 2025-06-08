# 🛡️ Deloitte Virtual Internship Cyber Sim Victory 🗿

## Cracked Deloitte’s Cyber Simulation by exposing a stealthy insider through Blue Team log forensics — SOC-mode: Activated.

In the ever-evolving battleground of cybersecurity, every challenge is an opportunity to sharpen your blade. Recently, I took on the **Deloitte Australia Cyber Security Virtual Internship Sim** hosted by [Forage](https://www.theforage.com/simulations/Deloitte%20Australia/cyber-c1e3) and what followed was a practical Blue Team drill that blended analytical thinking, threat detection and digital defense.

![Cover](https://github.com/user-attachments/assets/9b8b3222-2196-4785-a3a6-76184bd15403) <br/>

## 👔 Deloitte: More Than Just Consulting

When you hear *Deloitte*, you might think of suits, spreadsheets, and boardroom strategy — but beneath that corporate polish lies a **formidable force in cyber defense**.

Deloitte is one of the “Big Four” firms — not just a consulting empire, but also a **global powerhouse in cybersecurity services**. Their cyber teams protect Fortune 500 clients, critical infrastructure, and nation-level systems with layered defense models, including advanced **Security Operations Centers (SOCs)**, **Incident Response**, and **Threat Hunting** services.

So when they drop a simulation like this? It’s not a gimmick. It’s a **blue team boot camp** — and I went in ready to flex.🗿

---

## 🧩 The Challenge: A Simulated Breach at Daikibo Industrials

In this simulation, I joined Deloitte’s virtual cyber team to respond to a high-severity breach involving **Daikibo Industrials**, a major manufacturing client whose internal telemetry dashboard had leaked sensitive operational data.

Their **status board**, a key internal asset, was hosted inside a VPN-protected intranet. Yet sensitive data found its way out. My mission?

1. **Determine** if an external attacker (internet-based) could’ve breached the dashboard.
2. **Inspect the web activity logs** to identify malicious or suspicious behavior.

What followed was a deep dive into digital forensics.

---

## 🧠 Blue Team Mindset: Detection Over Exploitation

Unlike red teaming, where you’re the attacker, **blue teaming is all about defense** — detecting threats, mitigating them, and preserving the integrity of systems. In this case, I stepped into the shoes of a SOC analyst: scouring logs, recognizing behavioral patterns, and isolating the threat vector before the damage escalates.

Think of it as a tactical blend of:

* 🕵️‍♂️ Log analysis
* 🔐 Authentication flow review
* 🧮 Anomaly detection
* 🚫 Access control verification

The key? Pattern recognition — and I was on it.

---

## 📁 The Evidence: Parsing the Web Requests Log

The core of this simulation lay in the `web_requests.log` file — a massive chunk of HTTP activity segmented by static internal IPs. The format captured everything from login attempts to API requests, mapped against timestamps and status codes.

I booted it into my code editor, scanned through suspicious time series, and began drawing my battle lines.

After inspecting several user sessions, one stood out:

![1](https://github.com/user-attachments/assets/97677aad-f003-4187-9470-695d4075c72b) <br/>

### 🚨 Suspicious User Detected:

**User ID:** `dBCm2JjBU815PB8zPDvKqv`

### 💡 Here’s What Gave It Away:

* ✅ Logged in like everyone else. Nothing unusual at first.
   <br/> ![3](https://github.com/user-attachments/assets/c499b2a6-05bb-4bdd-a9a9-a2cc4ebdca71) <br/>

* 🤔 Then, a sequence of **automated API requests** began — hitting all factory endpoints.
* ⏱️ The pattern? **Punctual**. Every hour. On the dot. No frontend elements were requested — no styles, no scripts, no human browsing indicators.
   <br/> ![4](https://github.com/user-attachments/assets/b91c6e79-1549-4187-b18d-24c08a12a521) <br/>

* 🤖 This was no human. This was **scripted access** — silent, persistent, and efficient.

A textbook case of either:

* A **compromised credential** being used in a scheduled script
* Or an **insider threat** automating unauthorized data exfiltration

My conclusion? **This user was scraping internal operational data without oversight.**

---

## 🔐 The Verdict

### ❓Q1: Can an attacker reach the dashboard directly from the internet?

🟢 **Answer:** No. The dashboard lives behind a **VPN-only internal intranet**. No direct access from external IPs — unless someone on the inside lets you in.

### ❓Q2: Who triggered the breach behavior?

🟢 **Answer:** `dBCm2JjBU815PB8zPDvKqv`
The only user displaying machine-like querying frequency, accessing factory endpoints without UI resource calls.

---

## 🧠 Skills Sharpened in the Simulation

This was more than checkbox training. It challenged me to think like a **SOC analyst** responding to a real incident:

* 🛡️ **Blue Team Threat Hunting**: Identifying TTPs (Tactics, Techniques, Procedures) of threat actors
* 📊 **Behavioral Analysis**: Detecting human vs. non-human patterns
* 🔍 **SIEM-style Log Analysis**: Manual inspection of web request logs and timestamps
* 🔐 **Authentication & Access Flow Understanding**: Mapping legitimate vs. suspicious logins

All self-paced, but brutally real in execution.

---

## 📜 Outcome: Certified, Battle-Tested & Logged In 🗿

After completing the challenge, I received a certificate and recognition for my cyber instincts — a solid addition to my profile and a true **testament to blue team readiness**.

This simulation gave me a taste of Deloitte's real-world expectations — and I left with more than a certificate. I left with sharpened instincts, deeper insights, and a stronger resolve to defend digital systems like a stone wall.🧱🗿

---

## 🗿 Final Words: SOC Like a Pro, Think Like a Threat

This wasn’t just a task — it was a **cyber puzzle with business impact**. I didn’t just click through it; I dissected it. I played the defender, the analyst, the firewall, and the log inspector — all rolled into one.

If you’re serious about cybersecurity, blue teaming, or working in SOC environments, **challenges like these are invaluable**.

So here’s to cracking one more simulation — and preparing for the real world ahead. 🔥
Let’s get back to the logs, Bub. The hunt never ends. 🧠🛡️

---

**📄 Add it to the Resume. <br/>
📌 Pin it to LinkedIn. <br/>
🗿 Carry the stone-cold energy forward.** <br/>

---
