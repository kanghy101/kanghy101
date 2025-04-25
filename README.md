# 안녕하세요
### 🛡️ Attack Flow (Mermaid.js)

### 🛡️ Attack Flow (Mermaid.js - clean version)

```mermaid
flowchart TD
    A[Initial Access: WebLogic RCE Exploit] --> B[Execution: .class payload and obfuscated PowerShell]
    B --> C[Payload Deployment: frpc.zip, la.zip, ct.zip, nmap.zip, index.asp]
    C --> D[Tool Activation: fs.exe, rev.ps1, unzip.exe]
    D --> E[Privilege Escalation: FileZilla login from 130 to 143]
    E --> F[Credential Dumping: mimi.zip to 150_infos to infos.zip]
    F --> G[Data Exfiltration: FTP transfer of infos.zip from 143]
    G --> H[Crypto Mining: xmrig launched from xm.zip]
    H --> I[Termination: xmrig process stopped on Oct 27, 2023]

