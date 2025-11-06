
<p align="center">
  <a href="https://usestrix.com/">
    <img src=".github/logo.png" width="150" alt="Strix Logo">
  </a>
</p>

<h1 align="center">
Strix
</h1>

<h2 align="center">هکرهای متن‌باز هوش مصنوعی برای امنیت اپلیکیشن‌های شما</h2>

<div align="center">

[![Python](https://img.shields.io/pypi/pyversions/strix-agent?color=3776AB)](https://pypi.org/project/strix-agent/)
[![PyPI](https://img.shields.io/pypi/v/strix-agent?color=10b981)](https://pypi.org/project/strix-agent/)
[![PyPI Downloads](https://static.pepy.tech/personalized-badge/strix-agent?period=total&units=INTERNATIONAL_SYSTEM&left_color=GREY&right_color=RED&left_text=Downloads)](https://pepy.tech/projects/strix-agent)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)

[![GitHub Stars](https://img.shields.io/github/stars/usestrix/strix)](https://github.com/usestrix/strix)
[![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?&logo=discord&logoColor=white)](https://discord.gg/J48Fzuh7)
[![Website](https://img.shields.io/badge/Website-usestrix.com-2d3748.svg)](https://usestrix.com)

</div>

:star: _از Strix خوشتان آمد؟ ستاره به ما بدهید تا توسعه‌دهندگان دیگر آن را کشف کنند!_

<br />

<div align="center">
<img src=".github/screenshot.png" alt="Strix Demo" width="800" style="border-radius: 16px; box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3), 0 0 0 1px rgba(255, 255, 255, 0.1), inset 0 1px 0 rgba(255, 255, 255, 0.2); transform: perspective(1000px) rotateX(2deg); transition: transform 0.3s ease;">
</div>

> [!TIP]
> **جدید!** Strix اکنون به طور یکپارچه با GitHub Actions و خطوط لوله CI/CD ادغام شده است. به طور خودکار در هر درخواست استخراج برای آسیب‌پذیری‌ها اسکن کنید و کد ناامن را قبل از رسیدن به تولید مسدود کنید!

---

## 🦉 نمای کلی Strix

Strix عامل‌های هوش مصنوعی خودمختاری هستند که دقیقاً مانند هکرهای واقعی عمل می‌کنند - کد شما را به صورت پویا اجرا می‌کنند، آسیب‌پذیری‌ها را پیدا می‌کنند و آنها را از طریق اثبات‌های مفهومی واقعی تأیید می‌کنند. برای توسعه‌دهندگان و تیم‌های امنیتی که نیاز به تست امنیتی سریع و دقیق بدون بار کار تست نفوذ دستی یا مثبت‌های کاذب ابزارهای تحلیل ایستا دارند، ساخته شده است.

- **مجموعه کامل ابزار هکر** از پیش ساخته شده
- **تیم‌های عامل** که با هم همکاری می‌کنند و مقیاس‌پذیر هستند
- **تأیید واقعی** با PoC، نه مثبت‌های کاذب
- **CLI مبتنی بر توسعه‌دهنده** با گزارش‌های قابل اجرا
- **اصلاح خودکار و گزارش‌دهی** برای تسریع اصلاح

---

### 🎯 موارد استفاده

- تشخیص و تأیید آسیب‌پذیری‌های حیاتی در برنامه‌های خود.
- انجام تست‌های نفوظ در ساعت‌ها نه هفته‌ها با گزارش‌های انطباقی.
- خودکارسازی تحقیقات باگ باونی و تولید PoC برای گزارش‌دهی سریع‌تر.
- اجرای تست‌ها در CI/CD برای مسدود کردن آسیب‌پذیری‌ها قبل از رسیدن به تولید.

---

### 🚀 شروع سریع

پیش‌نیازها:
- Docker (در حال اجرا)
- Python 3.12+
- کلید ارائه‌دهنده LLM (یا یک LLM محلی)

```bash
# نصب
pipx install strix-agent

# پیکربندی ارائه‌دهنده هوش مصنوعی
export STRIX_LLM="openai/gpt-5"
export LLM_API_KEY="your-api-key"

# اجرای ارزیابی امنیتی
strix --target ./app-directory
```

اولین اجرا تصویر Docker sandbox را دریافت می‌کند. نتایج در `agent_runs/<run-name>` ذخیره می‌شوند.

### ☁️ میزبانی ابری

می‌خواهید راه‌اندازی را رد کنید؟ نسخه میزبانی شده ابری ما را امتحان کنید: **[usestrix.com](https://usestrix.com)**

## ✨ ویژگی‌ها

### 🛠️ ابزارهای امنیتی عامل

- **🔌 پراکسی کامل HTTP** - دستکاری و تحلیل کامل درخواست/پاسخ
- **🌐 اتوماسیون مرورگر** - مرورگر چند تب برای تست XSS، CSRF، جریان‌های احراز هویت
- **💻 محیط‌های ترمینال** - پوسته‌های تعاملی برای اجرای دستور و تست
- **🐍 زمان اجرای Python** - توسعه و تأیید بهره‌برداری سفارشی
- **🔍 شناسایی** - OSINT خودکار و نقشه‌برداری از سطح حمله
- **📁 تحلیل کد** - قابلیت‌های تحلیل ایستا و پویا
- **📝 مدیریت دانش** - یافته‌های ساختاریافته و مستندات حمله

### 🎯 تشخیص جامع آسیب‌پذیری

- **کنترل دسترسی** - IDOR، ارتقاء سطح دسترسی، دور زدن احراز هویت
- **حملات تزریق** - SQL، NoSQL، تزریق دستور
- **سمت سرور** - SSRF، XXE، نقص‌های deserialize
- **سمت کلاینت** - XSS، آلودگی نمونه اولیه، آسیب‌پذیری‌های DOM
- **منطق کسب‌وکار** - شرایط مسابقه، دستکاری جریان کار
- **احراز هویت** - آسیب‌پذیری‌های JWT، مدیریت جلسه
- **زیرساخت** - پیکربندی‌های نادرست، سرویس‌های در معرض دید

### 🕸️ گراف عامل‌ها

- **جریان‌های توزیع‌شده** - عامل‌های تخصصی برای حملات و دارایی‌های مختلف
- **تست مقیاس‌پذیر** - اجرای موازی برای پوشش جامع سریع
- **هماهنگی پویا** - عامل‌ها با هم همکاری می‌کنند و کشفیات را به اشتراک می‌گذارند


## 💻 مثال‌های استفاده

```bash
# تحلیل پایگاه کد محلی
strix --target ./app-directory

# بررسی امنیتی مخزن
strix --target https://github.com/org/repo

# ارزیابی برنامه وب
strix --target https://your-app.com

# تست سفیدخانه چند هدفه (کد منبع + برنامه مستقر)
strix -t https://github.com/org/app -t https://your-app.com

# تست چند محیط به صورت همزمان
strix -t https://dev.your-app.com -t https://staging.your-app.com -t https://prod.your-app.com

# تست متمرکز با دستورالعمل‌ها
strix --target api.your-app.com --instruction "اولویت‌بندی تست احراز هویت و مجوزها"

# تست با اعتبارنامه‌ها
strix --target https://your-app.com --instruction "تست با اعتبارنامه: testuser/testpass. تمرکز بر ارتقاء سطح دسترسی و دور زدن کنترل دسترسی."
```

### ⚙️ پیکربندی

```bash
export STRIX_LLM="openai/gpt-5"
export LLM_API_KEY="your-api-key"

# اختیاری
export LLM_API_BASE="your-api-base-url"  # اگر از مدل محلی استفاده می‌کنید، مثلاً Ollama, LMStudio
export PERPLEXITY_API_KEY="your-api-key"  # برای قابلیت‌های جستجو
```

[📚 مشاهده مدل‌های پشتیبانی شده هوش مصنوعی](https://docs.litellm.ai/docs/providers)

### 🤖 حالت بدون رابط

Strix را به صورت برنامه‌نویسی بدون رابط کاربری تعاملی با استفاده از پرچم `-n/--non-interactive` اجرا کنید - عالی برای سرورها و وظایف خودکار. CLI یافته‌های آسیب‌پذیری لحظه‌ای را چاپ می‌کند و گزارش نهایی قبل از خروج. با کد غیر صفر خروج می‌کند وقتی آسیب‌پذیری‌ها پیدا می‌شوند.

```bash
strix -n --target https://your-app.com --instruction "تمرکز بر آسیب‌پذیری‌های احراز هویت و مجوزها"
```

### 🔄 CI/CD (GitHub Actions)

Strix را می‌توان به خط لوله شما اضافه کرد تا با یک workflow سبک GitHub Actions، تست امنیتی را روی درخواست‌های استخراج اجرا کند:

```yaml
name: strix-penetration-test

on:
  pull_request:

jobs:
  security-scan:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4

      - name: نصب Strix
        run: pipx install strix-agent

      - name: اجرای Strix
        env:
          STRIX_LLM: ${{ secrets.STRIX_LLM }}
          LLM_API_KEY: ${{ secrets.LLM_API_KEY }}

        run: strix -n -t ./
```

## 🏆 پلتفرم سازمانی

پلتفرن مدیریت شده ما فراهم می‌کند:

- **📈 داشبوردهای اجرایی**
- **🧠 مدل‌های سفارشی‌سازی شده دقیق**
- **⚙️ ادغام CI/CD**
- **🔍 اسکن مقیاس بزرگ**
- **🔌 ادغام با سوم‌جانبان**
- **🎯 پشتیبانی سازمانی**

[**دریافت نسخه نمایشی سازمانی →**](https://usestrix.com)

## 🔒 معماری امنیتی

- **ایزوله‌سازی کانتینر** - همه تست‌ها در محیط‌های Docker sandbox اجرا می‌شوند
- **پردازش محلی** - تست‌ها به صورت محلی اجرا می‌شوند، هیچ داده‌ای به سرویس‌های خارجی ارسال نمی‌شود

> [!WARNING]
> فقط سیستم‌هایی را تست کنید که مالک آنها هستید یا مجوز تست دارید. شما مسئول استفاده اخلاقی و قانونی از Strix هستید.

## 🤝 مشارکت

ما مشارکت جامعه را خوشامد می‌گوییم! راه‌های مختلفی برای مشارکت وجود دارد:

### مشارکت در کد
راهنمای مشارکت [Contributing Guide](CONTRIBUTING.md) را برای جزئیات ببینید:
- راه‌اندازی محیط توسعه
- اجرای تست‌ها و بررسی کیفیت
- ارسال درخواست‌های pull
- دستورالعمل‌های سبک کد

### مجموعه ماژول‌های دستور
در مجموعه ماژول‌های تخصصی دستور برای عامل‌های هوش مصنوعی ما کمک کنید:
- تکنیک‌های تست پیشرفته برای آسیب‌پذیری‌ها، چارچوب‌ها و فناوری‌ها
- برای راهنمایی‌ها به [مستندات ماژول‌های دستور](strix/prompts/README.md) مراجعه کنید
- از طریق [درخواست‌های pull](https://github.com/usestrix/strix/pulls) یا [مسائل](https://github.com/usestrix/strix/issues) ارسال کنید

## 🌟 پروژه را پشتیبانی کنید

**از Strix خوشتان آمد؟** به ما یک ⭐ در GitHub بدهید!

## 👥 به جامعه ما بپیوندید

سؤال دارید؟ باگ پیدا کردید؟ می‌خواهید مشارکت کنید؟ **[به دیسکورد ما بپیوندید!](https://discord.gg/J48Fzuh7)**

</div>
```
