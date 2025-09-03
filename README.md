# Snort 3 Intrusion Detection Practice
Snort 3 入侵偵測實作

---------

<h2>Outline 簡介</h2>

This project demonstrates the installation, configuration, and rule writing of Snort 3 on a Kali Linux virtual machine. The focus is on detecting ICMP traffic (ping) using custom rules, observing real-time alerts, and understanding the differences between Snort 2 and Snort 3 configuration structures.

本專題展示了在 Kali Linux 虛擬機中安裝、設定並撰寫 Snort 3 規則的過程。重點在於透過自訂規則偵測 ICMP 流量 (ping)，觀察即時警示，並理解 Snort 2 與 Snort 3 在組態上的差異。

---------
<h2>Key Learning Outcomes 主要學習成果</h2>

* Install Snort 3 on Linux. (安裝 Snort 3 於 Linux)

* Configure Snort rules and configuration files. (設定 Snort 規則與組態檔)

* Write custom Snort rules (ICMP detection). (撰寫自訂 Snort 規則 (ICMP 偵測))

* Test rules and observe alerts in the console. (測試規則並於終端機觀察警示)

---------

<h2>Tools and Concepts Covered 涵蓋工具與概念</h2>

<div align="center">
</p>

| Aspect <br/>(面向) | Learning content and purpose <br/>(學習內容與目的) |
| ----------------- | ----------------------------------------------- |
| Intrusion Detection <br/>(入侵偵測) | Install and configure Snort 3 for packet inspection. <br/>(安裝並設定 Snort 3 以進行封包檢測) |
| Custom Rule Writing <br/>(自訂規則撰寫) | Write ICMP rules to detect ping requests. <br/>(撰寫 ICMP 規則以偵測 ping 請求) |
| Configuration Management <br/>(組態管理) | Modify `snort.lua` to include custom rules. <br/>(修改 `snort.lua` 以加入自訂規則) |
| Network Security Testing <br/>(網路安全測試) | Perform controlled ping tests to trigger alerts. <br/>(執行受控的 ping 測試以觸發警示) |
| Practical Security Thinking <br/>(資安實務思維) | Understand detection workflows and alert logging. <br/>(理解偵測流程與警示紀錄方式) |
</div>
<br/>

---------


<h2>Materials and Methods 材料與方法</h2>

[Environment]
* Oracle VM VirtualBox (VirtualBox 虛擬機)</b>
* Kali Linux OS (Kali Linux 作業系統)</b>
* Cisco Packet Tracer 8.2.2 </b>

[Tasks]
* Configure a Named Extended ACL (設定命名延伸 ACL)</b>
* Verify ACL Configuration (驗證 ACL 設定)</b>
* Apply the ACL on the Interface (在介面上套用 ACL)</b>
* Test the ACL Implementation (測試 ACL 實作)</b>

---------

<h2>Practice 實踐</h2>

<p align="center">
<b>Task 1: Configure a Named Extended ACL<br/>(設定命名延伸 ACL)</b><br/>
<img src="https://i.imgur.com/OAxFGYt.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 2: Verify ACL Configuration<br/>(驗證 ACL 設定)</b><br/>
<img src="https://i.imgur.com/Nws9sQv.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 3: Apply the ACL on the Interface<br/>(在介面上套用 ACL)</b><br/>
<img src="https://i.imgur.com/3Zaz1Hh.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 4-1: PC1 to Server1 & Server2</b><br/>
<img src="https://i.imgur.com/PFXcRvZ.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 4-2: PC2 to Server1 & Server2</b><br/>
<img src="https://i.imgur.com/4gAecmw.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 4-3: PC3 to Server1 & Server2</b><br/>
<img src="https://i.imgur.com/mp6TlYd.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


---------
<h2>Results 成果展示</h2>

This project successfully demonstrated the use of extended IPv4 Access Control Lists (ACLs) to enforce fine-grained traffic restrictions across a simulated enterprise network. By applying a named ACL on the router interface, we controlled access to different services based on both the source device and the destination server.

本專題成功展示了如何使用 延伸 IPv4 ACL 來在模擬企業網路中進行細緻的流量限制。透過在路由器介面套用命名 ACL，我們能根據 來源端設備 與 目的伺服器 來管控不同服務的存取。

Key results included:<br/>主要成果如下：</b><br/>

* PC1 was blocked from accessing the HTTP/HTTPS services of both servers, ensuring restricted web access.<br/>
  (PC1 被阻擋存取兩台伺服器的 HTTP/HTTPS 服務，確保網頁存取受限)</b>

* PC2 was blocked from FTP access, simulating file transfer limitations.<br/>
  (PC2 被阻擋 FTP 存取，模擬檔案傳輸限制)</b>

* PC3 was restricted from ICMP (ping) traffic, preventing basic connectivity checks.<br/>
  (PC3 被限制 ICMP (ping) 流量，避免進行連線測試)</b>

* Other legitimate traffic was permitted, ensuring normal network operations.<br/>
  (其他合法流量則被允許，確保正常的網路運作)</b>
  <br/>

Through these steps, the lab highlighted how ACLs provide a layered approach to network security, enabling administrators to enforce policies that align with organizational needs. This exercise also strengthened skills in router configuration, verification commands, and troubleshooting within a controlled Packet Tracer environment.

透過這些操作，本專題強調了 ACL 如何提供 分層式的網路安全防護，協助管理員依照組織需求制定政策。本次實作同時強化了在 路由器設定、驗證指令及故障排除 方面的實務能力，並在 Packet Tracer 環境下提供安全的學習與測試平台。

<p align="center"> <b>Command Differences<br/>(指令差異)</b> </p>

| Command <br/>(指令)     | Description <br/>(說明)                                                                                                                                                             | 中文說明                                                         |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| `show access-lists`   | Displays all ACL rules with **sequence numbers**. Sequence numbers define the processing order of ACL entries and allow easier modifications (e.g., inserting or deleting rules). | 顯示所有 ACL 規則，並附帶**序號**。序號決定 ACL 規則的處理順序，也方便後續修改（例如插入或刪除特定規則）。 |
| `show running-config` | Displays the device’s current configuration file, including ACLs, but **without sequence numbers**. The ACL rules are shown only as part of the full configuration.               | 顯示設備目前的設定檔，其中包含 ACL，但**不會顯示序號**。ACL 規則僅作為整體設定的一部分被列出。        |

---------

<h2>Reference 參考</h2>

[UniSQ] [CSC8520 - Securing Networks](https://handbook-guide.unisq.edu.au/course/2025/CSC8520)
<br/>
