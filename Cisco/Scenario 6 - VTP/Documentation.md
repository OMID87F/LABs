# 🔹استفاده از VTP برای توزیع VLANها
---
## 🔹محیط کار و توپولوژی
---
![[Topology.png]]
- **Cisco Packer Tracer**⬆️
---


## 🔹هدف
---
- با **استفاده از** VTP کار **تعریف و توزیع VLAN**ها رو متمرکز کنیم.
    
- **هدف** از این سناریو اینه که **کاربرد پروتکل** VTP رو ببینیم.
---


## 🔹اقدامات و کانفیگ‌ها
---
#### 🔸سوئیچ VTP Server
![[VTP - Server.png]]
- تعریف VTP⬆️

![[VTP - Server - VLAN.png]]
- تعریف VLANها⬆️

![[VTP - Server - Trunk.png]]
- تعریف پورت‌های Trunk⬆️

#### 🔸سوئیچ‌های VTP Client
![[VTP - Clients.png]]
- تعریف VTP⬆️

![[VTP - Clients - Trunk.png]]
- تعریف پورت‌ Trunk⬆️

![[VTP - Clients - Access VLAN.png]]
- تعریف پورت‌‌های Access⬆️

#### 🔸سوئیچ VTP Transparent
![[VTP - Transparent.png]]
- تعریف VTP⬆️

![[VTP - Transparent - Trunk.png]]
- تعریف پورت‌های Trunk⬆️
---


## 🔹راستی آزمایی
---
![[Monitoring - Clients.png]]
- توزیع شدن VLANها بین سوئیچ‌های Client✅

![[Monitoring - Transparent.png]]
- توزیع نشدن  VLANها به سوئیچ‌ Transparent✅
---


## 🔹مشکل
---
- **مشکل**ی نبود✅
---


## 🔹نتیجه
---
>سناریو **موفقیت‌آمیز** بود✅

- درسته سناریو تمرینی بود؛ ولی VTP در **مقیاس بزرگ** خیلی مهمه‼️
---
