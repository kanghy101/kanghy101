# 안녕하세요
### 🛡️ Attack Flow (Mermaid.js)

```mermaid
flowchart TD
    A[🛠️ Initial Access<br>WebLogic RCE Exploit] --> B[☠️ Execution<br>`.class` payload + Power-shell]
    B --> C[📦 Payload Deployment<br>frpc.zip, la.zip, ct.zip, nmap.zip, index.asp]
    C --> D[⚙️ Tool Activation<br>fs.exe, rev.ps1, unzip.exe]
    D --> E[🔐 Privilege Escalation<br>FileZilla login (130→143)]
    E --> F[🧠 Credential Dumping<br>mimi.zip → 150_infos → infos.zip]
    F --> G[📤 Data Exfiltration<br>FTP (infos.zip from 143)]
    G --> H[⛏️ Crypto Mining<br>xmrig started from xm.zip]
    H --> I[🧯 Termination<br>xmrig ended on Oct 27, 2023]
