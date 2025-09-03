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

Successfully installed and verified Snort 3 on Kali Linux.

Configured custom ICMP detection rules in icmp.rules and integrated them into snort.lua.

Executed Snort with console output and confirmed real-time alerts triggered by ICMP packets (ping).

Demonstrated understanding of Snort 3 rule structure and differences from Snort 2 configuration.

成功在 Kali Linux 上安裝並驗證 Snort 3。

在 icmp.rules 中設定 自訂 ICMP 偵測規則，並整合至 snort.lua。

使用終端機輸出模式執行 Snort，並確認 即時警示 在 ICMP 封包 (ping) 時觸發。

展示對 Snort 3 規則結構及其與 Snort 2 組態差異的理解。

---------

<h2>Reference 參考</h2>

[UniSQ] [CSC8520 - Securing Networks](https://handbook-guide.unisq.edu.au/course/2025/CSC8520)
<br/>
