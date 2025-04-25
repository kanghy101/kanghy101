# 안녕하세요
### 🎯 Simulated APT Attack Flow (Mermaid.js - realistic style)

```mermaid
flowchart TD
    A[Recon Stage: External scan identifies vulnerable WebLogic] --> B[Initial Access: RCE exploited via crafted .class payload]
    B --> C[Persistence Setup: index.asp webshell dropped + unzip.exe deployed]
    C --> D[Lateral Tooling: Tools staged (frpc.zip, la.zip, ct.zip, nmap.zip)]
    D --> E[Command & Control: fs.exe + rev.ps1 retrieved from GitHub repo]
    E --> F[Internal Pivot: FileZilla used for lateral move (130 -> 143)]
    F --> G[Privilege Escalation: Mimikatz-style dump via mimi.zip → infos.zip]
    G --> H[Exfiltration: FTP channel used to export credential dump]
    H --> I[Post-Exploitation: xm.zip unpacked → xmrig miner launched]
    I --> J[Cleanup/Exit: xmrig activity ends Oct 27, traces remain minimal]


