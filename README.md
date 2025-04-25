# 안녕하세요
### Simulated APT Attack Flow (Mermaid.js - final stable version)

```mermaid
flowchart TD
    A[Recon Stage - Vulnerable WebLogic Identified] --> B[Initial Access - RCE Exploited Using Malicious Java Class]
    B --> C[Persistence Established - Webshell and Dropper Deployed]
    C --> D[Tooling Deployed - frpc zip la zip ct zip nmap zip]
    D --> E[Command and Control - fs exe and rev ps1 from Remote Repo]
    E --> F[Lateral Movement - FileZilla Used from Host 130 to 143]
    F --> G[Privilege Escalation - Credential Dump Using mimi zip and infos zip]
    G --> H[Exfiltration - Data Sent Out via FTP Channel]
    H --> I[Crypto Mining - xmrig Deployed and Executed]
    I --> J[Cleanup and Exit - Activity Ceased on October 27]



