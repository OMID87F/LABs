# 🔹راه‌اندازی Hotspot و Queue برای کارگاه کامپیوتر
---
## 🔹محیط کار و توپولوژی
---
![[Shariati - Workstation- Rack.jpg]]
![[Shariati - Workstation.jpg]]
- **Shariati Computer Workstation**⬆️

![[WinBox.png]]
- **WinBox**⬆️

![[hAP mini.jpg]]
- **hAP mini**⬆️

![[Topology.png]]
- **Cisco Packet Tracer** (*Just for Topology view*)⬆️
---


## 🔹هدف
---
- با **استفاده از** سرویس **Hotspot** و **Queue** تنظیماتی رو اعمال کنیم که:
	
	1. در`Hotspot`:
		1. ادمین‌ شبکه **فقط** از طریق **یک** `MAC Address`و` IP Address` بتونه وارد بشه!
			
		2. دانش‌آموزا از shared user استفاده کنن! (28 نفر)
		
	2. در`Queues`:
		1. ادمین شبکه **همیشه** `8M` بگیره و **بتونه** به نهایت پهنای‌باند هم برسه!
			
		2. دانش‌آموزا هم **همیشه** `8M` بگیرن اما **نتونن** بیشتر بگیرن؛ و باهم برابر باشن (`pcq`)!
	
- **هدف** از این سناریو اینه که یک **کار واقعی** رو داخل یک **محیط واقعی** اجرا کنیم‼️
---


## 🔹اقدامات و کانفیگ‌ها
---
#### 🔸راه‌اندازی Hotspot
![[Shariati - Hotspot - Server.png]]
1. راه‌اندازی خود Hotspot Server⬆️

![[Shariati - Hotspot - Server Profile.png]]
![[Shariati - Hotspot - Server Profile - Login.png]]
2. تنظیم Server Profile⬆️

![[Shariati - Hotspot - User Profiles.png]]
3. ساخت User Profileها⬆️

![[Shariati - Hotspot - Users.png]]
4. ساخت خود Userها⬆️

#### 🔸راه‌اندازی Queueها
![[Shariati - Queues - Total.png]]
1. ساخت Total⬆️

![[Shariati - Queues - Admin - General.png]]
![[Shariati - Queues - Admin - Advanced.png]]
2.ساخت Admin⬆️

![[Shariati - Queues - Students - General.png]]
![[Shariati - Queues - Students - Advanced.png]]****
3. ساخت Students⬆️
---


## 🔹راستی آزمایی
---

1. تست شرط‌های Login ادمین⬆️


2. تست پهنای‌باندها⬆️ 
---



## 🔹مشکل
---
- **مشکل**‌م این بود که مرورگر باز نمیشد و **صفحه Login** نمیومد؛ حتی اگه`DNS Name` رو دستی میزدم!🛑
    
- **راه‌حل**‌ی نداشت؛ چون فهمیدم بجای `shariati` نوشته بودم `sharaiti`✅
---


## 🔹نتیجه
---
>سناریو موفقیت‌آمیز بود✅
---