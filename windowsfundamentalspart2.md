# windowsfundamentalspart2

> Easy | Windows Fundamentals | Date Completed: 4/28/26

---

## Task 1 - Introduction

> Read above and start the virtual machine



---

## Task 2 - System Configuration

> What is the name of the service that lists Systems Internals as the manufacturer?

PsShutdown

> Whom is the Windows license registered to?

Windows User

> What is the command for Windows Troubleshooting?

C:\Windows\System32\control.exe /name Microsoft.Troubleshooting

> What command will open the Control Panel? (name of .exe only)

control.exe

### 📸 Screenshot (System Configuration Proof)
<img width="957" height="921" alt="image" src="https://github.com/user-attachments/assets/5e02094c-9d64-4061-844f-e9f6de01969f" />

<img width="956" height="922" alt="image" src="https://github.com/user-attachments/assets/1b3fe8ca-568b-473f-a54b-41f1d04ca9be" />

### Key Concepts
- msconfig is used for troubleshooting startup/services
- Services can reveal installed tools (useful for detection)
- Control Panel and troubleshooting tools are accessible via commands

---

## Task 3 - Change UAC Settings

> What is the command to open User Account Control Settings?

id="g4h1k8" UserAccountControlSettings.exe

### Key Concepts
- UAC controls privilege elevation
- Lower UAC = higher security risk

---

## Task 4 - Computer Management

> What is the command to open Computer Management?

compmgmt.msc

> At what time every day is the GoogleUpdateTaskMachineUA task configured to run?

6:15 AM

> What is the name of the hidden share?

sh4r3dF0Ld3r

### 📸 Screenshot (Task Scheduler / Shares Proof)
<img width="955" height="917" alt="image" src="https://github.com/user-attachments/assets/1e1b7f30-c1b7-464b-ae54-ee93dc27216c" />

<img width="954" height="915" alt="image" src="https://github.com/user-attachments/assets/b8f6e6e5-db71-437d-890d-b75fed213dc4" />

### Key Concepts
- Task Scheduler automates processes (persistence vector)
- Shared folders can expose sensitive data
- Hidden shares (ending in $) are commonly abused

---

## Task 5 - System Information

> What is the command to open System Information?

msinfo32.exe

> What is listed under System Name?

THM-WINFUN2

> Under Environment Variables, what is the value for ComSpec?

%SystemRoot%\system32\cmd.exe

### Key Concepts
- System Information shows hardware + OS data
- Environment variables define system behavior
- Useful for enumeration during investigations

---

## Task 6 - Resource Monitor

> What is the command to open Resource Monitor?

resmon.exe

### 📸 Screenshot (Resource Monitoring Proof)
<img width="958" height="915" alt="image" src="https://github.com/user-attachments/assets/43f26c43-e4c6-4c81-bbbe-6e8480f025e7" />

### Key Concepts
- Resource Monitor shows CPU, memory, disk, network usage
- Useful for detecting abnormal processes

---

## Task 7 - Command Prompt

> In System Configuration, what is the full command for Internet Protocol Configuration?

id="r9v3f6" C:\Windows\System32\cmd.exe /k %windir%\system32\ipconfig.exe

> For the ipconfig command, how do you show detailed information?

id="s5w1h8" ipconfig /all

### 📸 Screenshot (Network Info Proof)
md id="t2x7j4" ![IPConfig Output](./images/task7-ipconfig.png) 

### Key Concepts
- ipconfig shows network configuration
- /all reveals detailed system networking info
- Used heavily in troubleshooting + incident response

---

## Task 8 - Registry Editor

> What is the command to open the Registry Editor?

id="u8y4k2" regedt32.exe

### 📸 Screenshot (Registry Access Proof - Important)
md id="v1z6n9" ![Registry Editor](./images/task8-registry.png) 

### Key Concepts
- Registry stores system + application settings
- Frequently targeted by malware for persistence

---

## Task 9 - Conclusion

> Completed Windows Fundamentals Part 2

id="w3a8c5" 

---

## Key Takeaways

- System Configuration helps analyze services and startup behavior
- Task Scheduler is a major persistence mechanism
- System Information aids in enumeration
- Resource Monitor helps detect abnormal activity
- Registry is critical for both system config and attacks

---

## Skills Demonstrated

- Windows system configuration analysis
- Task scheduling and shared resource inspection
- System and environment variable enumeration
- Resource monitoring and troubleshooting
- Registry interaction

---

## Tools Used

- msconfig
- compmgmt.msc
- msinfo32
- resmon
- cmd / ipconfig
- Registry Editor

---
