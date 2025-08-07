# Eagle Donation Platform

## Overview

The **Eagle Donation Platform** is a modern, secure, and multilingual donation platform built to support innovation and technological advancement. It integrates with ZarinPal for secure payment processing and supports Persian, English, and Chinese languages. The platform features a sleek user interface with light/dark theme support, real-time statistics, donation badges, and secure payment options (both gateway and direct payment methods).

This repository contains a single HTML file (`index.html`) that includes all the necessary HTML, CSS, and JavaScript to run the platform. It uses Tailwind CSS for styling, supports multiple languages, and includes advanced security features like rate limiting and input sanitization.

---

## Features

- **Multilingual Support**: Persian, English, and Chinese languages with RTL/LTR support.
- **Theme Toggle**: Switch between light and dark themes.
- **Secure Payments**: Integration with ZarinPal for gateway and direct payment methods.
- **Real-time Statistics**: Displays total donations, supporters, and progress toward goals.
- **Donation Badges**: Earn badges based on donation amounts.
- **Live Activity Feed**: Shows recent donations with animations.
- **Transaction History**: Fetches transaction details via ZarinPal's GraphQL API.
- **Responsive Design**: Optimized for both desktop and mobile devices.
- **Security Features**: Includes rate limiting, XSS protection, and CSRF prevention.

---

## Installation and Setup

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, etc.).
- A ZarinPal merchant account for payment processing (optional for testing).
- A Telegram bot token and chat ID for notifications (optional).

### Setup Instructions
1. **Download the File**: Obtain the `index.html` file from this repository.
2. **Host the File**: Place the `index.html` file on a web server or open it directly in a browser for testing.
3. **Configure ZarinPal**:
   - Obtain a ZarinPal Merchant ID and Access Token from your ZarinPal dashboard.
   - Update the `ZARINPAL_MERCHANT_ID`, `ZARINPAL_ACCESS_TOKEN`, and `ZARINPAL_TERMINAL_ID` variables in the JavaScript section of `index.html`.
4. **Configure Telegram Notifications** (optional):
   - Set up a Telegram bot and obtain the `TELEGRAM_BOT_TOKEN` and `TELEGRAM_CHAT_ID`.
   - Update these variables in the JavaScript section of `index.html`.
5. **Run the Platform**:
   - Open `index.html` in a browser or host it on a server.
   - The platform will load with a welcome modal and support Persian as the default language.

### Notes
- The platform uses CDN-hosted Tailwind CSS and Google Fonts (Vazirmatn, Roboto, Noto Sans SC) for styling and typography.
- Ensure an internet connection for CDN dependencies and ZarinPal API calls.
- For production use, host the file on a secure server with HTTPS.

---

## Usage

1. **Select Language**: Use the language selector in the top-right corner to switch between Persian, English, and Chinese.
2. **Choose Donation Amount**: Select a predefined amount or enter a custom amount.
3. **Enter Details**: Provide optional name, email, and message for the donation.
4. **Select Payment Method**: Choose between gateway payment (card) or direct payment (bank contract).
5. **Complete Payment**: Follow the prompts to complete the payment via ZarinPal.
6. **View Statistics and Badges**: Monitor real-time stats and earned badges in the sidebar.

---

## Technologies Used
- **HTML5**: For structure and content.
- **CSS3 with Tailwind CSS**: For responsive and modern styling.
- **JavaScript**: For interactivity, payment processing, and API integration.
- **ZarinPal API**: For secure payment processing and transaction history.
- **LocalStorage**: For persisting configuration and donation statistics.

---

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Make changes to the `index.html` file.
3. Submit a pull request with a clear description of your changes.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgements
- Built with ❤️ by Hamid Yarali.
- Thanks to ZarinPal for their reliable payment API.
- Uses Tailwind CSS and Google Fonts for styling.

---

# پلتفرم دونیت ایگل

## بررسی اجمالی

**پلتفرم دونیت ایگل** یک پلتفرم مدرن، امن و چندزبانه برای جمع‌آوری کمک‌های مالی است که به منظور حمایت از نوآوری و پیشرفت فناوری طراحی شده است. این پلتفرم با زرین‌پال برای پردازش پرداخت امن ادغام شده و از زبان‌های پارسی، انگلیسی و چینی پشتیبانی می‌کند. دارای رابط کاربری زیبا با پشتیبانی از تم روشن/تیره، آمار بلادرنگ، نشان‌های دونیت و گزینه‌های پرداخت امن (درگاه پرداخت و پرداخت مستقیم) است.

این مخزن شامل یک فایل HTML (`index.html`) است که تمام کدهای HTML، CSS و جاوااسکریپت لازم برای اجرای پلتفرم را در خود جای داده است. از Tailwind CSS برای استایل‌دهی استفاده شده و از چندین زبان و ویژگی‌های امنیتی پیشرفته مانند محدود کردن نرخ و پاکسازی ورودی‌ها پشتیبانی می‌کند.

---

## ویژگی‌ها

- **پشتیبانی چندزبانه**: پشتیبانی از زبان‌های پارسی، انگلیسی و چینی با جهت‌گیری راست‌به‌چپ و چپ‌به‌راست.
- **تغییر تم**: امکان جابجایی بین تم‌های روشن و تیره.
- **پرداخت امن**: ادغام با زرین‌پال برای روش‌های پرداخت درگاه و مستقیم.
- **آمار بلادرنگ**: نمایش مجموع کمک‌ها، تعداد حامیان و پیشرفت به سمت اهداف.
- **نشان‌های دونیت**: کسب نشان‌ها بر اساس مبلغ کمک.
- **فید فعالیت زنده**: نمایش کمک‌های اخیر با انیمیشن.
- **تاریخچه تراکنش‌ها**: دریافت جزئیات تراکنش‌ها از طریق API GraphQL زرین‌پال.
- **طراحی پاسخگو**: بهینه‌سازی شده برای دسکتاپ و موبایل.
- **ویژگی‌های امنیتی**: شامل محدود کردن نرخ، محافظت در برابر XSS و پیشگیری از CSRF.

---

## نصب و راه‌اندازی

### پیش‌نیازها
- یک مرورگر وب مدرن (کروم، فایرفاکس، سافاری و غیره).
- حساب پذیرنده زرین‌پال برای پردازش پرداخت (اختیاری برای تست).
- توکن ربات تلگرام و آیدی چت برای اعلان‌ها (اختیاری).

### دستورالعمل‌های راه‌اندازی
1. **دانلود فایل**: فایل `index.html` را از این مخزن دریافت کنید.
2. **میزبانی فایل**: فایل `index.html` را روی یک سرور وب قرار دهید یا مستقیماً در مرورگر برای تست باز کنید.
3. **پیکربندی زرین‌پال**:
   - یک شناسه پذیرنده و توکن دسترسی از داشبورد زرین‌پال دریافت کنید.
   - متغیرهای `ZARINPAL_MERCHANT_ID`، `ZARINPAL_ACCESS_TOKEN` و `ZARINPAL_TERMINAL_ID` را در بخش جاوااسکریپت فایل `index.html` به‌روزرسانی کنید.
4. **پیکربندی اعلان‌های تلگرام** (اختیاری):
   - یک ربات تلگرام راه‌اندازی کنید و `TELEGRAM_BOT_TOKEN` و `TELEGRAM_CHAT_ID` را دریافت کنید.
   - این متغیرها را در بخش جاوااسکریپت فایل `index.html` به‌روزرسانی کنید.
5. **اجرای پلتفرم**:
   - فایل `index.html` را در مرورگر باز کنید یا روی سرور میزبانی کنید.
   - پلتفرم با یک مودال خوش‌آمدگویی بارگذاری می‌شود و زبان پارسی به صورت پیش‌فرض تنظیم شده است.

### نکات
- پلتفرم از Tailwind CSS میزبانی‌شده در CDN و فونت‌های گوگل (وزیرمتن، روبوتو، نوتو سانس SC) برای استایل و تایپوگرافی استفاده می‌کند.
- برای وابستگی‌های CDN و تماس‌های API زرین‌پال به اتصال اینترنت نیاز است.
- برای استفاده در محیط تولید، فایل را روی یک سرور امن با HTTPS میزبانی کنید.

---

## استفاده

1. **انتخاب زبان**: از انتخابگر زبان در گوشه بالا-راست برای جابجایی بین پارسی، انگلیسی و چینی استفاده کنید.
2. **انتخاب مبلغ دونیت**: یک مبلغ از پیش تعیین‌شده انتخاب کنید یا مبلغ دلخواه وارد کنید.
3. **وارد کردن جزئیات**: نام، ایمیل و پیام اختیاری برای دونیت وارد کنید.
4. **انتخاب روش پرداخت**: بین پرداخت درگاه (کارت) یا پرداخت مستقیم (قرارداد بانکی) انتخاب کنید.
5. **تکمیل پرداخت**: دستورات را برای تکمیل پرداخت از طریق زرین‌پال دنبال کنید.
6. **مشاهده آمار و نشان‌ها**: آمار بلادرنگ و نشان‌های کسب‌شده را در نوار کناری مشاهده کنید.

---

## فناوری‌های استفاده‌شده
- **HTML5**: برای ساختار و محتوا.
- **CSS3 با Tailwind CSS**: برای استایل‌دهی مدرن و پاسخگو.
- **جاوااسکریپت**: برای تعامل، پردازش پرداخت و ادغام API.
- **API زرین‌پال**: برای پردازش پرداخت امن و تاریخچه تراکنش‌ها.
- **LocalStorage**: برای ذخیره پیکربندی و آمار دونیت.

---

## مشارکت
از مشارکت استقبال می‌شود! برای مشارکت:
1. مخزن را فورک کنید.
2. تغییرات را در فایل `index.html` اعمال کنید.
3. یک درخواست کشیدن با توضیحات واضح از تغییرات خود ارسال کنید.

---

## مجوز
این پروژه تحت مجوز MIT منتشر شده است. برای جزئیات به فایل [LICENSE](LICENSE) مراجعه کنید.

---

## تقدیر و تشکر
- ساخته‌شده با ❤️ توسط حمید یرعلی.
- تشکر از زرین‌پال برای API پرداخت قابل اعتمادشان.
- استفاده از Tailwind CSS و فونت‌های گوگل برای استایل‌دهی.

---

# 雄鹰捐款平台

## 概述

**雄鹰捐款平台** 是一个现代、安全且支持多语言的捐款平台，旨在支持创新和技术进步。它与ZarinPal集成以实现安全支付处理，并支持波斯语、英语和中文。该平台具有优雅的用户界面，支持明暗主题、实时统计、捐款徽章和安全的支付选项（网关支付和直接支付方式）。

该存储库包含一个单一的HTML文件（`index.html`），其中包括运行平台所需的所有HTML、CSS和JavaScript代码。它使用Tailwind CSS进行样式设计，支持多种语言，并包括速率限制和输入清理等高级安全功能。

---

## 功能

- **多语言支持**：支持波斯语、英语和中文，带RTL/LTR支持。
- **主题切换**：在明暗主题之间切换。
- **安全支付**：与ZarinPal集成，支持网关和直接支付方式。
- **实时统计**：显示总捐款、支持者数量和目标进度。
- **捐款徽章**：根据捐款金额获得徽章。
- **实时活动流**：展示带有动画的近期捐款。
- **交易历史**：通过ZarinPal的GraphQL API获取交易详情。
- **响应式设计**：针对桌面和移动设备优化。
- **安全功能**：包括速率限制、XSS防护和CSRF预防。

---

## 安装与设置

### 先决条件
- 现代网页浏览器（Chrome、Firefox、Safari等）。
- ZarinPal商户账户用于支付处理（测试时可选）。
- Telegram机器人令牌和聊天ID用于通知（可选）。

### 设置说明
1. **下载文件**：从该存储库获取`index.html`文件。
2. **托管文件**：将`index.html`文件放置在Web服务器上，或直接在浏览器中打开进行测试。
3. **配置ZarinPal**：
   - 从ZarinPal仪表板获取商户ID和访问令牌。
   - 在`index.html`的JavaScript部分更新`ZARINPAL_MERCHANT_ID`、`ZARINPAL_ACCESS_TOKEN`和`ZARINPAL_TERMINAL_ID`变量。
4. **配置Telegram通知**（可选）：
   - 设置Telegram机器人并获取`TELEGRAM_BOT_TOKEN`和`TELEGRAM_CHAT_ID`。
   - 在`index.html`的JavaScript部分更新这些变量。
5. **运行平台**：
   - 在浏览器中打开`index.html`或在服务器上托管。
   - 平台将加载欢迎模态框，默认语言为波斯语。

### 注意事项
- 平台使用CDN托管的Tailwind CSS和Google Fonts（Vazirmatn、Roboto、Noto Sans SC）进行样式和排版。
- 需要互联网连接以支持CDN依赖和ZarinPal API调用。
- 生产环境中，建议在支持HTTPS的安全服务器上托管文件。

---

## 使用方法

1. **选择语言**：使用右上角的语言选择器在波斯语、英语和中文之间切换。
2. **选择捐款金额**：选择预定义金额或输入自定义金额。
3. **输入详情**：为捐款提供可选的姓名、电子邮件和消息。
4. **选择支付方式**：在网关支付（银行卡）或直接支付（银行合同）之间选择。
5. **完成支付**：按照提示通过ZarinPal完成支付。
6. **查看统计和徽章**：在侧边栏中监控实时统计和获得的徽章。

---

## 使用技术
- **HTML5**：用于结构和内容。
- **CSS3与Tailwind CSS**：用于现代和响应式样式设计。
- **JavaScript**：用于交互、支付处理和API集成。
- **ZarinPal API**：用于安全支付处理和交易历史。
- **LocalStorage**：用于持久化配置和捐款统计。

---

## 贡献
欢迎贡献！要参与贡献：
1. Fork存储库。
2. 对`index.html`文件进行更改。
3. 提交一个带有清晰更改描述的拉取请求。

---

## 许可证
该项目采用MIT许可证发布。详情请见[LICENSE](LICENSE)文件。

---

## 致谢
- 由Hamid Yarali用❤️构建。
- 感谢ZarinPal提供的可靠支付API。
- 使用Tailwind CSS和Google Fonts进行样式设计。