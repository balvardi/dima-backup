
```markdown
# Dima Backup

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Dima Backup** یک پلاگین ساده و امن برای وردپرس است که به شما کمک می‌کند تمام فایل‌ها و دیتابیس سایت خود را بصورت زیپ‌بندی شده و قابل انتقال خارج کنید. این پلاگین بخصوص برای انتقال سایت‌های وردپرس از محیط لوکال به سرور آنلاین بسیار مناسب است.

---

## ✅ ویژگی‌ها

- 🔧 **انتقال سایت وردپرس از لوکال به سرور**
- 📦 **ایجاد فایل زیپ از تمام فایل‌های سایت**
- 💾 **صادرات دیتابیس بصورت SQL**
- 🚀 **ایجاد فایل `import.php` برای وارد کردن دیتابیس در سرور مقصد**
- 🕒 **اجرای Async با AJAX بدون Timeout**
- 📈 **نوار پیشرفت بصورت Live**
- 🎲 **اسم فایل زیپ بصورت رندوم (بدون از دست دادن فایل‌های قبلی)**

---

## ⚙️ نحوه نصب

1. پوشه `dima-backup` را داخل پوشه `wp-content/plugins/` قرار دهید.
2. در پنل ادمین وردپرس به بخش **افزونه‌ها > افزونه‌های نصب شده** بروید.
3. پلاگین **Dima Backup** را فعال کنید.
4. به بخش **ابزارها > Dima Backup** بروید و تنظیمات مورد نظر را انجام دهید.

---

## 📋 نحوه استفاده

1. به بخش **ابزارها > Dima Backup** بروید.
2. اطلاعات دیتابیس سرور مقصد را وارد کنید:
   - هاست دیتابیس
   - نام کاربری
   - رمز عبور
   - نام دیتابیس
3. روی دکمه **شروع بک‌آپ** کلیک کنید.
4. صبر کنید تا نوار پیشرفت کامل شود.
5. فایل‌های زیر در پوشه `wp-content/exports/` ایجاد می‌شوند:
   - `backup_xxxxxxxx.zip`
   - `database.sql`
   - `import.php`

> 💡 فایل `import.php` را در روت سرور آنلاین آپلود کنید و در مرورگر باز کنید تا دیتابیس وارد شود.

---

## 📁 ساختار پوشه

```
/wp-content/plugins/dima-backup/
├── dima-backup.php       ← اصل پلاگین
├── assets/
│   └── script.js         ← مدیریت AJAX و UI
└── includes/
    └── handlers.php      ← مدیریت مراحل بک‌آپ
```

---

## ⛔ شرایط لازم

- وردپرس 5.0 یا بالاتر
- PHP 7.2 یا بالاتر
- دسترسی نوشتنی به پوشه `wp-content/exports/`

---

## 📌 رفع مشکلات متداول

### ❗ خطای `Internal Server Error`
- دلیل: محدودیت زمان اجرای PHP
- راه حل: در `php.ini` این مقادیر را افزایش دهید:
  ```ini
  max_execution_time = 300
  memory_limit = 256M
  ```

### ❗ فایل‌های دیگر ساخته نمی‌شوند
- دلیل: عدم دسترسی نوشتنی به پوشه `exports/`
- راه حل: دسترسی (`chmod`) پوشه `wp-content/exports/` را به `755` تغییر دهید.

---

## 🤝 مشارکت در پروژه

همه مشارکت‌ها و ارسال pull request خوش آمد است!  
اگر ایده‌ای برای بهبود پلاگین دارید، مثل افزودن قابلیت‌های جدید، اصلاح باگ‌ها یا بهینه‌سازی کد، خوشحال می‌شویم که در توسعه این پروژه همراه ما باشید.

---

## 📜 مجوز

این پروژه تحت [مجوز MIT](LICENSE) منتشر شده است.

---

## 📬 تماس با من

نویسنده: **دیما**  
ایمیل: dima@example.com  
وب‌سایت: [https://example.com](https://example.com)  
گیت‌هاب: [github.com/dimawp](https://github.com/dimawp)
```

---

## 📁 فایل LICENSE (MIT)

همچنین یک فایل `LICENSE` با محتوای زیر اضافه کن:

```
MIT License

Copyright (c) 2025 دیما

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## ✅ نکته مهم:
در قسمت **تماس با من** اطلاعات خودت رو جایگزین کن (مثل ایمیل، وب‌سایت و گیت‌هاب).

---
