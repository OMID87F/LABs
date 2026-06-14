# 🔹راه‌اندازی`OSPF`بین 5 روتر
---
## 🔹محیط کار و توپولوژی
---
![[Module 4 - OSPF/Topology.png]]
- **Packet Tracer** *(just for topology view)* ⬆️

![[Module 4 - OSPF/Sources/Winbox.png]]
- **WinBox**⬆️

![[Module 4 - OSPF/Sources/VMWare.png]]
- **VMWare**⬆️
---


## 🔹هدف
---
- با **استفاده از** پروتکل `OSPF` ارتباط بین **5 روتر**مون رو برقرار کنیم؛ 4 روتر باید بتونن **از طریق** روتر`R1` به اینترنت **دسترسی** داشته باشن! (و کلاینت‌ها)
    
- **هدف** از این سناریو اینه که `OSPF`رو خیلی **کلی** تمرین کنیم✅
---


## 🔹اقدامات و کانفیگ‌ها
---
#### 1️⃣تعریف`Router ID`ها
![[Router ID (1).png]]
![[Router ID (2).png]]
![[Router ID (3).png]]
![[Router ID (4).png]]
![[Router ID (5).png]]
>در **ساده**‌ترین حالت و بدون تنظیمات اضافی‼️


#### 2️⃣ساخت`Instance`ها
![[Instances (1).png]]
![[Instances (2).png]]
![[Instances (3).png]]
![[Instances (4).png]]
![[Instances (5).png]]
>روتر`R1`**نیاز** به گزینه`Originate Dafault`داره چون یه اینترفیسش به **اینترنت** وصله؛ روترهای`R4`و`R5`هم به`Redistribute`**نیاز** دارن تا **LANها**ی خودشون رو معرفی کنن‼️


#### 3️⃣ساخت`Area`ها
![[Areas (1).png]]
![[Areas (2).png]]
![[Areas (3).png]]
![[Areas (4).png]]
![[Areas (5).png]]
>روترهای`R2`و`R3`باید **دو Area** داشته باشن چون **ABR** هستن‼️


#### 4️⃣ساخت`Interface Template`ها
![[Interface Templates (1).png]]
![[Interface Templates (2).png]]
![[Interface Templates (3).png]]
![[Interface Templates (4).png]]
![[Interface Templates (5).png]]
>گزینه`Network Type`برای **همه** میتونه`ptp`باشه چون **مستقیما** بهم دیگه وصل شدن‼️


#### 5️⃣تعریف`src-nat`برای `R1`,`R4`,`R5`
![[srcnat (1).png]]
![[srcnat (2).png]]
![[srcnat (3).png]]
>روتر`R1`بخاطر **اینترنت** نیاز به`srcnat`داره؛ روترهای`R4`و`R5`هم بخاطر **LANها**شون‼️
---


## 🔹راستی آزمایی
---
![[Pathping (1).png]]
![[Pathping (2).png]]
- دستور`pathping` بین کلاینت‌ها⬆️

![[Tracert-2-Internet(1).png]]
![[Tracert-2-Internet(2).png]]
- دستور`tracert`به سمت اینترنت⬆️
---


## 🔹مشکل
---
- **مشکل**م این بود که روی **ورژن 3** کار نمیکردن🛑
    
- **راه‌حل**‌ هم این بود که یکم **سرچ** کردم و فهمیدم`OSPFv3`مختص`IPv6`ساخته شده‼️😅
---


## 🔹نتیجه
---
>سناریو **موفقیت‌آمیز** بود✅
---