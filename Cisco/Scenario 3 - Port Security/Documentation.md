# 🔹راه‌اندازی Port Security روی L2 Switch
---
## 🔹محیط کار و توپولوژی
---
![[ Scenario 3 - Port Security/Topology.png]]
- **Cisco Packet Tracer** (*Just for Topology view*)⬆️
---


## 🔹هدف
---
- با **استفاده از** **قابلیت Port Security** کاری کنیم تا از طریق`gig 0/1`تنها **3تا MAC Address** بتونن از`SW-0`عبور کنن؛ از **حالت`restrict`** استفاده میکنیم ولی خب سرور Log نداریم‼️
    
- **هدف** از این سناریو اینه که **کلی و پایه‌ای** مبحث Port Security رو **تمرین** کنیم✅
---


## 🔹اقدامات و کانفیگ‌ها
---
![[Port Security - All in One.png]]
>تمام اقدامات⬆️
---


## 🔹راستی آزمایی
---
![[Show Port-Security (1).png]]
- دستور `show port-security interface g0/1`⬆️

![[Show Port-Security (2).png]]
- دستور `show port-security address`⬆️

![[Ping - C1&C2.png]]
- تست ارتباط **کلاینت‌های 1 و 2** با لپ‌تاپ‌ها⬆️

![[Ping - C3&C4.png]]
- تست ارتباط **کلاینت‌های 3 و 4** با لپ‌تاپ‌ها⬆️
---


## 🔹مشکل
---
>**مشکل**ی نبود✅ 
---


## 🔹نتیجه
---
>سناریو **موفقیت‌آمیز** بود✅
---