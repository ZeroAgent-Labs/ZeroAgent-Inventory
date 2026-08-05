# Zero Agent Inventory Collector

Lightweight, Agentless IT Asset Management for Windows. Zero dependencies, Zero installation, Privacy-first.

Managing IT assets shouldn't require installing heavy background agents or setting up complex servers. This portable PowerShell script collects detailed hardware, software, and security information from offline/air-gapped Windows PCs without leaving a trace. Output is saved locally as a structured JSON file.

Perfect for MSPs, Sysadmins, and One-Person IT departments who need quick, secure audits.

## ✅ Features

*   **Portable:** No installation required. Runs from a USB drive or network share.
*   **Agentless:** Does not run in the background. Runs only when you execute it.
*   **Safe & Private:** 100% open-source PowerShell. No data is sent to the Internet.
*   **Comprehensive Data Collected:**
    *   **System:** Hostname, OS, CPU, RAM, GPU, Serial Number.
    *   **Storage:** Disk usage, Total/Free GB (detect low disk space instantly).
    *   **Network:** IP Address (IPv4), MAC Address.
    *   **Software:** Full list of installed applications.
    *   **Security:** BitLocker encryption status, Antivirus/Defender signature dates, Windows Update pending reboots, Local Administrators list.

## ⚙️ Installation & Usage

**Step 1: Download**
Download `Collect-PC-Inventory.ps1` to your USB drive or local machine.

**Step 2: Collect Data (Client Side)**
Run the script on the target Windows PC. 
*(Note: Administrator privileges are required to retrieve BitLocker and security statuses. If run as a standard user, security details will be marked as unknown).*

Open PowerShell as Administrator and run:
```powershell
powershell.exe -ExecutionPolicy Bypass -File .\Collect-PC-Inventory.ps1
```
📊 Don't want to parse raw JSON? (Optional GUI)
If you are managing dozens of machines, reading raw JSON files manually can be painful. My team uses a pre-compiled GUI viewer we built that aggregates these JSONs into static, filterable HTML dashboards.

If you want to save time building your own parser, you can grab the standalone GUI tool here:
👉 [Get Zero Agent Viewer on Gumroad]

Live sample report (dummy data): https://zeroagent-labs.github.io/za-sample-report/

Workflow guide: https://zeroagent-labs.github.io/blog/
