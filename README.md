# 🛡️ VEXRMC Security Bot

![Version](https://img.shields.io/badge/version-1.1.2-blue)
![Discord](https://img.shields.io/badge/discord-bot-7289DA)
![Security](https://img.shields.io/badge/security-advanced-red)
![License](https://img.shields.io/badge/license-MIT-green)
![Logo](/assets/TC.gif)
> 🔐 **VEXRMC** คือ Security Bot สำหรับ Discord  
> ป้องกัน **Raid / Nuke / Spam / Abuse** แบบระดับ Production  
> รองรับ **Multi-Guild (แยก config ต่อ server)**

---

## 📑 Table of Contents

- [🧠 แนวคิดหลัก](#-แนวคิดหลัก)
- [🚀 การติดตั้ง](#-การติดตั้ง)
- [⚙️ Setup Commands](#️-setup-commands)
- [🛡️ Security Systems](#️-security-systems)
- [👥 Whitelist & Trusted](#-whitelist--trusted)
- [🔐 Permission System](#-permission-system)
- [📜 Logging System](#-logging-system)
- [📊 Monitoring](#-monitoring)
- [🔁 Automation](#-automation)
- [🧠 Setup Flow](#-setup-flow)
- [📁 Project Structure](#-project-structure)

---

## 🧠 แนวคิดหลัก

- ทุกคำสั่งทำงานแบบ **Per-Guild**
- ใช้ `getGuildConfig(guildId)` แยกข้อมูล
- ❌ ห้ามใช้ใน DM
- 🔐 ตรวจ permission ทุกคำสั่ง

### 🧩 ระบบหลัก

- 👑 Admin Role
- 🔁 Fallback Role
- 🚫 Whitelist
- 🛡️ Trusted Role

---

## 🚀 การติดตั้ง

### 1️⃣ เชิญบอท (OAuth2)

https://discord.com/oauth2/authorize?client_id=1373550516961017876&permissions=8&integration_type=0&scope=bot+applications.commands
---

### 2️⃣ Setup ครั้งแรก

```bash id="setup_cmd"
/setup all
```
### ตรวจสอบ config:
```
/config
```
⚙️ Setup Commands
```
/setup all
/setup adminrole
/setup fallbackrole
/setup logchannel
/setup safechannel_add
/setup safechannel_remove
/setup safechannel_list
/setup createlog
```

### 🛡️ Security Systems
🚨 Anti-Raid
```
/antiraid set
```
> threshold: จำนวน user
> 
> action: kick / ban / mute
> 
> window: เวลา

💣 Anti-Nuke
```
/antinuke set
```
ป้องกัน:
> ลบ channel
> 
> ลบ role
> 
> mass ban
> 
> webhook spam

🔒 Lockdown
```
/lockdown
```
> ล็อกทุก channel

⚠️ Panic Mode
```
/panic confirm:PANIC
```
> เปิดระบบป้องกันฉุกเฉิน

## 👥 Whitelist & Trusted
### Whitelist
```
/whitelist add
/whitelist remove
/whitelist list
```
> 👉 ไม่โดนลงโทษ

### Trusted Role
```
/trustedrole add
/trustedrole remove
/trustedrole list
```
> 👉 bypass บางระบบ

### 🔐 Permission System
```
/permission view
/permission set
/permission clear
```
> 👉 กำหนดว่า: ใครใช้คำสั่งอะไรได้
> 
> /permission set all @role ถือว่าใช้ อุนญาติ ทุกคำสั่งให้ @role

## 📜 Logging System
```
/log view
/log set
/log enable
/log disable
/log reset
```
📌 ประเภท log
security
message
member
role
audit
### 📊 Monitoring
```
/status
/stats
/audit
```
> 👉 ดู:
```uptime```
```latency```
```logs การใช้งาน```
```เหตุการณ์ทั้งหมด```

## 🔁 Automation
### บอทจะทำงานอัตโนมัติ:
```🔍 ตรวจ spam```
```🔗 ตรวจ link```
```🚨 ตรวจ raid```
```💣 ตรวจ nuke```
```🧹 auto clean```
```♻️ auto restore บางส่วน```

## ⚠️ หมายเหตุสำคัญ
❗ อย่าให้ admin role ผิดคน

❗ อย่าลืม whitelist ตัวเอง

❗ อย่า reset config โดยไม่ backup

❗ ตรวจ permission bot ให้ครบ

## 🏢 ผู้พัฒนา
### TechAsRMC Co., Ltd. 
