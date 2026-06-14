# 🔹راه‌اندازی EtherChannel بین 2 سوئیچ
---
## 🔹محیط کار و توپولوژی
---
![[ Scenario 2 - EtherChannel/Topology.png]]
- Cisco Packer Tracer⬆️
---


## 🔹هدف
---
- با **استفاده از** پروتکل PAgP بین 2 سوئیچ‌‌مون با 2 تا پورت یک EtherChannel راه‌‌اندازی کنیم؛ و VLAN رو هم از توش عبور بدیم!
    
- **هدف** از این سناریو اینه که یه کار **کوچیک ولی کاربردی** رو انجام داده باشیم.
---


## 🔹اقدامات و کانفیگ‌ها
---
![[VLAN - SW1.png]]
![[VLAN - SW2.png]]
1. ساخت `VLAN` و `access` کردن پورت⬆️

![[Etherchannel+Trunk - SW1.png]]
![[Etherchannel+Trunk - SW2.png]]
1. ساخت`EtherChannel`و تغییر به`trunk`⬆️

![[Ports+Mode - SW1.png]]
![[Ports+Mode - SW2.png]]
1. اضافه‌کردن`پورت‌ها`و انتخاب `mode`⬆️
---


## 🔹راستی آزمایی
---
![[ Scenario 2 - EtherChannel/Sources/Ping.png]]
- بررسی ارتباط کلاینت‌ها⬆️

![[Eth Summary.png]]
- دستور`show etherchannel summary`⬆️
---


## 🔹مشکل
---
- **مشکل**م این بود که ترتیب **دستورات** رو خوب یادم نمیموند🛑
    
- **راه‌حل‌**ش هم دیدن **ویدیو آموزشی** بود؛ و اینکه ترتیبش زیاد **مهم نبود**!✅
---


## 🔹نتیجه
---
>سناریو موفقیت‌آمیز بود✅
---