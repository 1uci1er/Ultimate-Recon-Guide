# Ultimate-Recon-Guide
<img src="https://github.com/user-attachments/assets/5784774f-0d0e-43fc-ab2d-cd0556c4b09d" alt="recon_icon" width="250" height="200" 
     src="https://media1.tenor.com/m/6ipiVGBsTIUAAAAd/scan-wow.gif" alt="scann_icon" width="200" height="200"/> 
     <img src="https://github.com/user-attachments/assets/64d6fe4f-9d73-47a4-999c-a5aca465ed6d" alt="Alt Text" width="400" />
<p>Image source <link>https://osintteam.blog</p>


## Ultimate Recon Tools Methodology for Bug Bounty Hunters

**Hello Hackers!**

I am your host and dost, **Aditya AKA (1uci1er)** — a passionate security researcher and bug hunter. Today, let’s dive deep into **Reconnaissance ("Recon")**, the foundation of a successful bug bounty hunter.

Recon is all about identifying assets, technologies, and potential vulnerabilities. It’s the key to uncovering critical bugs. In this guide, I’ll walk you through my ultimate recon methodology step-by-step. So, gear up, and let’s get hacking! 🚀

---

### Step 1: **Scope Review** 📏

Before anything else, **review the in-scope targets**. This ensures you focus only on authorized assets and stay ethical (nobody wants legal trouble!).

**Example Scope:**
- `target.com`
- `sub.domain.target.com`

---

### Step 2: **Subdomain Enumeration** 🔍

The first step in gathering intel is identifying all possible subdomains. Many tools are available for this purpose, both manual and automated.

**Recommended Tool:**
- [bbot](https://github.com/blacklanternsecurity/bbot.git) 🔧

This tool provides a comprehensive subdomain enumeration technique. To use:
```bash
bbot -d target.com
```

---

### Step 3: **Check Alive Subdomains** 🚪

Once you have a list of subdomains, verify which ones are alive. For this, I highly recommend `httpx` — a fantastic tool from the ProjectDiscovery team.

**Tool:** [httpx](https://github.com/projectdiscovery/httpx.git) 🏦

**Command:**
```bash
cat subdomain.txt | httpx -silent -o alive_subdomains.txt
```

---

### Step 4: **Crawling Alive Subdomains** 🛠

After identifying live subdomains, use a crawler to gather additional endpoints for further analysis. A fabulous tool for this is `katana` by ProjectDiscovery. It’s like Google’s spider but for bug hunters.

**Tool:** [katana](https://github.com/projectdiscovery/katana.git) 🕸

---

### Step 5: **Screenshotting** 🔍

Visual reconnaissance can save a lot of time. Automate taking screenshots of all live subdomains to identify potentially interesting targets.

**Recommended Tool:**
- [EyeWitness](https://github.com/RedSiege/EyeWitness) 📷

This tool automates the process and stores screenshots neatly for analysis.

---

**Icons, humor, and useful tools make recon a fun and effective process! Let’s get hunting and uncover those bugs like pros.** 🔎

