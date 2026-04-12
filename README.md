# 🧠 SelfSurvey

> **Self-host your surveys. Own your data. The free alternative to Google Forms.**

A fully self-hosted survey platform built on LimeSurvey, deployed on free hosting with duplicate response prevention, token-based access control, and unlimited responses — no paid plans needed.

---

## 🌐 Live Demo

👉 [https://surveybynomi.great-site.net/limesurvey/index.php/458434](https://surveybynomi.great-site.net/limesurvey/index.php/458434)

---

## ✨ Features

- ✅ **100% Free** — No paid plans, no subscriptions, no limits
- ✅ **Duplicate Prevention** — Token-based access ensures one response per person
- ✅ **Public or Closed Access** — Choose who can respond
- ✅ **Unlimited Responses** — No monthly caps like Google Forms
- ✅ **30+ Question Types** — Likert scale, multiple choice, rating, text and more
- ✅ **Data Ownership** — Your data stays on your own server
- ✅ **SPSS/CSV Export** — Ready for academic research and analysis
- ✅ **No Google Account Required** — Fully independent platform

---

## 📊 Why SelfSurvey over Google Forms?

| Feature | Google Forms | SelfSurvey |
|---|---|---|
| Cost | Free (with limits) | 100% Free |
| Response limit | Limited | Unlimited |
| Duplicate prevention | Basic (Google login) | Token-based (bulletproof) |
| Data ownership | Google owns it | You own it |
| Question types | Limited | 30+ types |
| SPSS export | ❌ | ✅ |
| Self-hosted | ❌ | ✅ |
| Academic research ready | ❌ | ✅ |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Survey Platform | LimeSurvey 6.16 (Community Edition) |
| Backend | PHP 8.3 |
| Database | MySQL |
| Hosting | InfinityFree (Free) |
| File Transfer | FileZilla FTP |

---

## 🚀 How to Deploy Your Own

### Prerequisites
- A free [InfinityFree](https://infinityfree.com) account
- [FileZilla](https://filezilla-project.org) FTP client
- [LimeSurvey Community Edition](https://community.limesurvey.org/downloads/)

### Step 1 — Set Up Hosting
1. Sign up at [infinityfree.com](https://infinityfree.com)
2. Create a hosting account and note your:
   - FTP Host
   - FTP Username & Password
   - MySQL Host, Username, Password

### Step 2 — Download LimeSurvey
1. Download the latest stable release from [community.limesurvey.org](https://community.limesurvey.org/downloads/)
2. Extract the ZIP file on your computer

### Step 3 — Upload via FTP
1. Open FileZilla
2. Connect using your FTP details (use IP address to avoid IPv6 issues)
3. Navigate to `htdocs` on the server
4. Upload the extracted `limesurvey` folder

### Step 4 — Run the Installer
1. Visit `yoursite.infinityfreeapp.com/limesurvey/admin`
2. Follow the installation wizard
3. Enter your MySQL database details
4. Create your admin account

### Step 5 — Create Your Survey
1. Log in to the admin panel
2. Click **"Create Survey"**
3. Add your questions
4. Configure participant settings
5. Activate and share!

---

## 🔐 Duplicate Prevention Setup

SelfSurvey uses LimeSurvey's powerful token system:

1. Go to **Survey Participants** → **Initialize Participant Table**
2. Add participants (name + email)
3. Click **"Generate Access Codes"**
4. Each participant gets a **unique one-time link**
5. After submission, the token is marked as used — permanently blocked

---

## 📁 Project Structure

```
limesurvey/
├── admin/          # Admin panel
├── application/    # Core application
├── themes/         # Survey themes
├── upload/         # Uploaded files
└── index.php       # Entry point
```

---

## 📸 Screenshots

### Admin Dashboard
> Create and manage surveys from a clean dashboard

### Survey View
> Clean, mobile-friendly survey interface for respondents

### Responses & Statistics
> Visual charts and exportable data for analysis

---

## 🤝 Use Cases

- 📚 **Academic Research** — Psychology studies, field research
- 🏫 **Education** — Student feedback, quizzes
- 🏢 **Business** — Customer feedback, employee surveys
- 🧪 **Psychology Studies** — Likert scales, rating questions
- 📊 **Data Collection** — Any structured data gathering

---

## ⚠️ Known Limitations

- InfinityFree does **not** support SSH/SFTP — use FTP with IPv4
- Free hosting has occasional downtime
- Email sending requires external SMTP configuration
- For production use, consider a paid VPS for better reliability

---

## 📄 License

This project uses [LimeSurvey Community Edition](https://github.com/LimeSurvey/LimeSurvey) which is licensed under **GPL-2.0**.

---

## 👤 Author

**Nomi**
- GitHub: [@nomi](https://github.com)
- Survey: [surveybynomi.great-site.net](https://surveybynomi.great-site.net)

---

## ⭐ Support

If you found this helpful, please give it a **star** ⭐ on GitHub!

> *Built with ❤️ as a free alternative to Google Forms*
