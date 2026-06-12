# ALMS-AI-Life-Management-System
An open-source life management system with 10 modules — from personal finance and smart bill reminders to OCR receipt scanning, ibadah tracking, and an AI chat assistant. Built on PHP Native + MySQL, zero framework dependency.

🌙 ALMS — AI Life Management System


Manage your dunya, don't let it manage you.



ALMS is an open-source, self-hosted life management system built with PHP Native + MySQL — no heavy frameworks, no monthly subscription. One login to manage your finances, bills, documents, vehicles, family, ibadah, and more — with an AI assistant built right in.


✨ Features

ModulFungsi📊 DashboardRingkasan kewangan, bil, ibadah & notifikasi dalam satu pandangan💰 KewanganRekod pendapatan & perbelanjaan, bajet bulanan, carta analisis🧾 BilJejak bil elektrik, air, internet — dengan status bayar/belum🤖 AI Smart ScanImbas resit & bil secara automatik menggunakan OCR🗂️ Dokumen DigitalSimpan salinan IC, sijil, polisi insurans dengan selamat🚗 KenderaanPantau roadtax, takaful & servis — dapat reminder sebelum tamat👨‍👩‍👧 KeluargaRekod ahli keluarga, jadual & kalendar acara🕌 IbadahLog solat, puasa, sedekah & zakat harian💬 AI AssistantChat pintar berkuasa OpenAI terus dalam sistem🔔 Notifikasi PintarReminder automatik untuk bil, roadtax & temujanji


🛠️ Tech Stack


Backend: PHP 7.4+ (Native, tanpa framework)
Database: MySQL via PDO
Frontend: Bootstrap 5 + Chart.js + Font Awesome
AI: OpenAI API (chat assistant)
OCR: ocr.space API (smart scan)
Server: XAMPP / Apache



🚀 Pemasangan (XAMPP Localhost)

1. Clone atau Download

bashgit clone https://github.com/username/alms.git

Atau extract ZIP ke dalam folder XAMPP htdocs:

C:\xampp\htdocs\alms

2. Start XAMPP

Buka XAMPP Control Panel → Start Apache dan MySQL.

3. Import Database


Buka http://localhost/phpmyadmin
Klik New → nama database: alms_db
Pilih alms_db → tab Import
Pilih fail database/alms_db.sql → klik Go


4. Konfigurasi

Edit config/config.php jika perlu:

php// Tambah API keys untuk fungsi AI
define('OPENAI_API_KEY', 'sk-xxxxx');   // AI Assistant
define('OCR_API_KEY',    'xxxxx');      // AI Smart Scan (ocr.space)

5. Akses Sistem

http://localhost/alms

6. Login Default

PerananEmailPasswordAdminadmin@alms.localadmin123Useruser@alms.localuser123


⚠️ Tukar password default selepas login pertama.




📁 Struktur Folder

alms/
├── config/          # Konfigurasi database & app
├── includes/        # Header, footer, auth, helper functions
├── assets/
│   ├── css/         # Stylesheet
│   ├── js/          # JavaScript
│   └── uploads/     # Dokumen & resit yang diupload
├── modules/         # 10 modul utama
│   ├── dashboard/
│   ├── finance/
│   ├── bills/
│   ├── scan/
│   ├── documents/
│   ├── vehicles/
│   ├── family/
│   ├── ibadah/
│   ├── assistant/
│   └── notifications/
├── admin/           # Panel admin
├── api/             # API endpoints (OCR, AI chat)
├── database/        # SQL schema
├── index.php        # Entry point
├── login.php
├── register.php
└── logout.php


🔒 Keselamatan


✅ Session-based authentication
✅ CSRF token pada semua form
✅ Password hashing dengan bcrypt
✅ PDO prepared statements (anti SQL Injection)
✅ htmlspecialchars pada semua output (anti XSS)
✅ .htaccess untuk menyekat akses terus ke folder config/



📸 Screenshots


(Tambah screenshot dashboard, modul kewangan, AI assistant di sini)




🗺️ Roadmap


 Versi mobile-responsive yang lebih baik
 Export laporan ke PDF
 Multi-user family sharing
 Integrasi dengan FPX / payment gateway Malaysia
 Dark mode



🤝 Sumbangan

Pull request amat dialu-alukan! Untuk perubahan besar, sila buka issue dahulu untuk berbincang.


Fork projek ini
Buat branch baru (git checkout -b feature/nama-feature)
Commit perubahan (git commit -m 'Add: nama feature')
Push ke branch (git push origin feature/nama-feature)
Buka Pull Request



📄 Lesen

Projek ini dilesenkan di bawah MIT License — bebas digunakan untuk projek peribadi mahupun komersial.


<div align="center">
Dibina dengan ❤️ untuk komuniti Malaysia

"Sesungguhnya Allah menyukai apabila seseorang dari kamu melakukan sesuatu pekerjaan, dilakukan dengan tekun dan sempurna."

</div>
