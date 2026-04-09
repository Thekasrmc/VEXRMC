# 🛡️ VEXRMC Security Bot

![Version](https://img.shields.io/badge/version-1.2.0-blue)
![Discord](https://img.shields.io/badge/discord-bot-7289DA)
![Security](https://img.shields.io/badge/security-advanced-red)
![Logo](/assets/TC.gif)
> 🔐 **VEXRMC** คือ Security Bot สำหรับ Discord  
> ป้องกัน **Raid / Nuke / Spam / Abuse** แบบระดับ Production  
> รองรับ **Multi-Guild (แยก config ต่อ server)**
> 
> **แนะนำ‼️** [EasyRMC Bot ช่วยให้ใช้การใช้ Serverใช้งานง่ายขึ้น มี คำสั่งให้ใช้มากมาย หากต้องการกดที่นี่เลย !!!](https://github.com/Thekasrmc/EasyRMC)


---

## 🚀 Quick Start (เริ่มใช้งานเร็ว)
### 1️⃣ เชิญบอท (OAuth2)

 ### https://discord.com/oauth2/authorize?client_id=1373550516961017876&permissions=8&integration_type=0&scope=bot+applications.commands
---

### 2️⃣ Setup ครั้งแรก

```bash id="setup_cmd"
/setup all หรือ /setup panel 
```
### 3️⃣ ตรวจสอบ สถานะ:
```
/config
```
### 🎛️ Setup Panel (แนะนำ)
```
/setup panel
```
> 👉 จะได้หน้าตั้งค่าแบบ interactive (embed + ปุ่ม)
> สามารถตั้งค่า:
> 
> ```Admin Role```
> ```Log Channel```
> ```Safe Channels```
> ```Trusted Roles```
> ```Whitelist```
> ```Security Systems```
> 
> ✅ ความพิเศษ
> มี Preview Diff ก่อน Save
> ต้องกด Confirm / Cancel
> ลดความผิดพลาดในการตั้งค่า

## 🛡️ Security Systems
🚨 Anti-Raid
```
/antiraid set
```
> ```threshold: จำนวน user```
> 
> ```action: kick / ban / mute```
> 
> ```window: เวลา```

💣 Anti-Nuke
```
/antinuke set
```
ป้องกัน:
> ```ลบ channel```
> ```ลบ role```
> ```mass ban```
> ```webhook spam```

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

## 🌐 Link Filter (Advanced)
### จัดการลิงก์:
```
/linkfilter view
/linkfilter set
/linkfilter allow_add
/linkfilter deny_add
/linkfilter test
```
### รองรับ:
> ```https://```
> ```www```
> ```discord.gg```
> ```discord.com/invite```
### ฟีเจอร์:
> ```Allowlist / Denylist```
> ```Bypass (role / channel / user)```
> ```Normalize domain```

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
### 📌 ประเภท log
```security```
```message```
```member```
```role```
```audit```
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
```♻️ auto restore บางกรณี```

## 🧠 Setup Flow (แนะนำ)
1. ```/setup all```
2. ```/setup panel```
ตั้ง:
3. ```Admin Role```
4. ```Log Channel```
5. ```เปิด Security Systems```
6. ```ทดสอบ /test```
## ⚠️ Important Notes
❗ อย่าให้ admin role ผิดคน

❗ อย่าลืม whitelist ตัวเอง

❗ อย่า reset config โดยไม่ backup

❗ ตรวจ permission bot ให้ครบ

## 🏢 Developer
### TechAsRMC Co., Ltd. 
