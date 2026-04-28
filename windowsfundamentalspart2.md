# windowsfundamentalspart2

> Easy | Windows Fundamentals | Date Completed: 

---

## Task 1 - Introduction

> Read above and start the virtual machine

id="a9f2k1" 

---

## Task 2 - System Configuration

> What is the name of the service that lists Systems Internals as the manufacturer?

id="b3m7x2" PsShutdown

> Whom is the Windows license registered to?

id="c8q4p9" Windows User

> What is the command for Windows Troubleshooting?

id="d1z6r5" C:\Windows\System32\control.exe /name Microsoft.Troubleshooting

> What command will open the Control Panel? (name of .exe only)

id="e5n2v7" control.exe

### 📸 Screenshot (System Configuration Proof)
md id="f7t9y3" ![System Configuration](./images/task2-msconfig.png) 

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

id="i2l5w6" compmgmt.msc

> At what time every day is the GoogleUpdateTaskMachineUA task configured to run?

id="j8o3c1" 6:15 AM

> What is the name of the hidden share?

id="k6p9s4" sh4r3dF0Ld3r

### 📸 Screenshot (Task Scheduler / Shares Proof)
md id="l0x7e2" ![Computer Management](./images/task4-compmgmt.png) 

### Key Concepts
- Task Scheduler automates processes (persistence vector)
- Shared folders can expose sensitive data
- Hidden shares (ending in $) are commonly abused

---

## Task 5 - System Information

> What is the command to open System Information?

id="m3q6v8" msinfo32.exe

> What is listed under System Name?

id="n7r2z5" THM-WINFUN2

> Under Environment Variables, what is the value for ComSpec?

id="o1s9b4" %SystemRoot%\system32\cmd.exe

### Key Concepts
- System Information shows hardware + OS data
- Environment variables define system behavior
- Useful for enumeration during investigations

---

## Task 6 - Resource Monitor

> What is the command to open Resource Monitor?

id="p4t8y1" resmon.exe

### 📸 Screenshot (Resource Monitoring Proof)
md id="q6u2d7" ![Resource Monitor](./images/task6-resmon.png) 

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
