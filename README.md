راه اندازی سرور فیلترشکن شخصی
----------------------------------------------------------------- 

ساخت یک سرور با سیستم عامل: Centos 7 x86 (or) Centos 7 x64

لاگین کردن به سرور با نرم افزار putty و اجرای دستور زیر:

cd /tmp/ && yum install git -y && git clone https://github.com/wikm360/wikm.git && cd Personal-vpn/ && sed -i -e 's/\r$//' centos7.sh && chmod 755 centos7.sh && ./centos7.sh 

دستورات زیر برای اضافه کردن کاربر به سرور:

useradd [username] - 
passwd [username]

نتونستم وصل بشم یا سرعتم کمه: 🔴
اگه روی ویندوز یا مک نتونستید کانکت بشید یا سرعت خوبی نداشتید اول مثل مراحلی که برای موبایل طی کردیم پروفایل رو دانلود میکنید.
بعد از لینک زیر نسخه آخر open vpn رو نصب میکنید و پروفایل دانلود شده رو میندازید داخلش.
https://openvpn.net/vpn-client/

محدود کردن تعداد کانکشن هر کاربر: 🔴
در حالت پیشفرض هر کاربر میتونه با یک اکانت روی چندین دستگاه به سرور وصل بشه.
اگه میخواید هر کاربر به طور هم زمان فقط روی یک دستگاه بتونه کانکت بشه و اگه دستگاه دوم کانکت شد به صورت خودکار دستگاه اول قطع بشه این کارو انجام بدید:
(اینکار بسیار مفیده و باعث میشه کاربر نتونه از اکانتش سو استفاده کنه)
برای اینکار کافیه در بخش Configuration روی گزینه Advanced VPN کلیک کنید
و گزینه Multiple Sessions per User رو خاموش کنید و تنظیمات رو آپدیت کنید.
در این صورت هر اکانت رو فقط روی یک دیوایس میشه استفاده کرد و اگه دیوایس دوم وصل بشه دیوایس اول قطع میشه.

تغییر پسورد ادمین سرور: 🔴
برای تغییر پسورد خود سرور کافیه بعد از وارد شدن به سرور از طریق نرم افزار putty دستور زیر رو تایپ کنید:
passwd root
و بعد پسورد جدید رو تایپ کنید.
(انجام اینکار برای افزایش امینت سرور ضروریه)

----------------------------------------------------------
سایت های خرید سرور مجازی:

https://parspack.com/

https://onlineserver.ir/

https://daryaserver.ir/

https://www.vps2day.com/

https://console.hetzner.cloud/projects

https://www.digitalocean.com/pricing/droplets#basic-droplets

-----------------------------------------------------------
🔵 لیست پورت ها:
443
587
53
21
22
80
123
143
3306
8080
54783
1194

---------------------------------------------------------------

منبع:

@AlefBeMedia

https://www.youtube.com/watch?v=1NfR6wrKTVA

