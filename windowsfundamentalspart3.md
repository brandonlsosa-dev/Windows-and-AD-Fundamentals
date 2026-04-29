# 🪟 Windows Fundamentals 3 — TryHackMe Notes

## 📌 Overview
This room covers core Windows security features including updates, antivirus, firewall, encryption, and recovery mechanisms used to protect systems.

---

## 🧠 Key Concepts

### 🔄 Windows Updates
- Provides security patches, bug fixes, and feature updates
- Cannot be permanently disabled (only postponed)
- Critical for vulnerability mitigation

**Key Insight:** Keeping systems updated is one of the highest ROI security practices

---

### 🛡️ Windows Security (Dashboard)
- Centralized interface for system protection
- Status indicators:
  - Green → Protected
  - Yellow → Action recommended
  - Red → Immediate attention required

---

### 🦠 Virus & Threat Protection
- Powered by Microsoft Defender Antivirus
- Provides real-time protection and scanning

**Important Setting:**
- Real-time protection should always be ON

[Screenshot Placeholder: Virus & Threat Protection Dashboard]

---

### 🔥 Firewall & Network Protection
- Blocks unauthorized access to the system
- Network profiles:
  - Domain
  - Private
  - Public (least trusted)

**Key Insight:** Public networks apply stricter rules for security

---

### 🌐 App & Browser Control
- Protects against malicious apps, files, and websites
- Uses Microsoft SmartScreen

---

### 🔐 Device Security
- Focuses on hardware-level protection

**Key Component:**
- Trusted Platform Module (TPM)
  - Securely stores cryptographic keys

---

### 💽 BitLocker (Disk Encryption)
- Encrypts entire disk to protect data at rest

**Requirements:**
- TPM recommended
- Without TPM → requires USB startup key

---

### 🧬 Volume Shadow Copy Service (VSS)
- Creates restore points and backups
- Enables file recovery and system restoration

---

## 🧪 Task Answers

Task 2: 5/3/2021  
Task 3: Virus & threat protection  
Task 4: Real-time protection  
Task 5: Public network  
Task 7: Trusted Platform Module  
Task 8: USB startup key  
Task 9: Volume Shadow Copy Service  

---

## 🧠 Real-World Takeaways

- Patch management is the first line of defense
- Antivirus misconfiguration is a common vulnerability
- Public network profiles reduce exposure on untrusted networks
- BitLocker protects against physical device compromise
- TPM is essential for modern endpoint security

---

## 🗂️ Suggested GitHub Structure

TryHackMe/  
└── Windows-Fundamentals/  
&nbsp;&nbsp;&nbsp;&nbsp;└── Windows-Fundamentals-3.md  

---

## 🚀 Portfolio Upgrade Ideas

- Add screenshots of:
  - Windows Security dashboard
  - Firewall settings
  - BitLocker configuration
- Include short reflections:
  - "What I learned" per section
- Optional:
  - PowerShell commands
  - SOC-related use cases
