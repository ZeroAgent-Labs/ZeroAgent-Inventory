# Zero Agent Inventory

## 💎 Professional Viewing & Management Tool
**Need a GUI to manage your collected data efficiently?** The Zero Agent Collector script is free, but the raw JSON output is difficult to handle. Access the pre-compiled **Zero Agent Viewer** for a beautiful, filtering-enabled dashboard and priority support.

👉 **[Get Zero Agent Viewer on Gumroad (Instant Download)](https://zeroagentlabs.gumroad.com/l/Zero-Agent-Viewer)**

---

Lightweight, Agentless IT Asset Management for Windows. Zero dependencies, Zero installation, Privacy-first.

### ❓ Why ZeroAgent?
Managing IT assets shouldn't require installing heavy agents or setting up complex servers. **ZeroAgent Inventory** is a portable PowerShell script that collects detailed hardware and software information from Windows PCs without leaving a trace.

Perfect for MSPs, Sysadmins, and One-Person IT departments who need quick audits.

### ✅ Features
* **Portable:** No installation required. Runs from a USB drive or network share.
* **Agentless:** Does not run in the background. Runs only when you execute it.
* **Safe & Private:** 100% open-source PowerShell. No data is sent to the Internet.
* **Comprehensive Data:**
    * **System:** Hostname, OS, CPU, RAM, GPU.
    * **Storage:** Disk usage, Total/Free GB (detect low disk space instantly).
    * **Network:** IP Address (IPv4), MAC Address.
    * **Software:** Full list of installed applications (analyzes Registry).

### ⚙️ Installation & Usage

#### Step 1: Download
Download `ZeroAgentCollector.ps1` from the file list above.

#### Step 2: Collect Data (Client Side)
Run the script on the target Windows PC (Administrator privileges recommended for full details).

```powershell
# Run via PowerShell
.\ZeroAgent_Collector.ps1
