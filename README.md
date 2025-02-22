<div align="center">
  <img alt="LOGO" src="https://raw.githubusercontent.com/Twentytwoaio/streamaio/refs/heads/main/img/logo.png" width="420" height="auto" />
</div>

# StreamAio: Aplikasi Live Streaming Multi-Window

**StreamAio** adalah aplikasi live streaming yang memungkinkan pengguna untuk melakukan siaran langsung ke berbagai platform seperti YouTube, Facebook, dan lainnya menggunakan protokol RTMP. Aplikasi ini berjalan di VPS (Virtual Private Server) dan mendukung streaming ke banyak platform sekaligus dengan fitur multi-window. StreamAio juga dilengkapi dengan fitur login dan riwayat streaming untuk memantau aktivitas siaran langsung.

<p align="center">
  <img alt="screenshot" src="https://raw.githubusercontent.com/Twentytwoaio/streamaio/refs/heads/main/img/screenshot.jpg" width="500px" height="auto" />
</p>

---

## ✨ Fitur Utama

- **Multi-Window Streaming:** Streaming ke beberapa platform sekaligus dalam satu aplikasi.
- **Dukungan Banyak Platform:** Bisa streaming ke YouTube, Facebook, dan platform lain yang mendukung RTMP.
- **Login Page:** Hanya pengguna terdaftar yang dapat mengakses aplikasi.
- **Riwayat Streaming:** Melacak dan menyimpan histori streaming.

---

## 📌 Cara Instalasi

> **Sebelum memulai**, pastikan Anda telah mengunggah kode ini ke repositori GitHub Anda sendiri.  
> Jika belum, ikuti langkah-langkah berikut:

### **1️⃣ Upload Kode ke GitHub**
Jika belum memiliki repositori GitHub, buat dan unggah kode dengan perintah berikut:

```bash
# Inisialisasi Git dan buat repositori baru
git init
git remote add origin https://github.com/GITHUB_USERNAME_ANDA/streamaio.git
git add .
git commit -m "Inisialisasi proyek StreamAio"
git branch -M main
git push -u origin main

### 1️⃣ **Siapkan Server**
Pastikan server/VPS Anda telah menginstal **Node.js**, **npm**, dan **FFmpeg** sebelum meng-clone repositori ini.

```bash
curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
sudo apt-get install -y nodejs npm
node -v
npm -v
```

### 2️⃣ **Install FFmpeg**
```bash
sudo apt-get update
sudo apt-get install -y ffmpeg
ffmpeg -version
```

### 3️⃣ **Install PM2**
```bash
npm install -g pm2
```

### 4️⃣ **Clone Repositori** *(Gantilah dengan URL repositori GitHub Anda!)*
```bash
git clone https://github.com/GITHUB_USERNAME_ANDA/streamaio/
cd streamaio
```

### 5️⃣ **Install Dependensi**
```bash
npm install
```

### 6️⃣ **Jalankan Aplikasi**
```bash
pm start
```
Atau menggunakan PM2:
```bash
pm install -g pm2
pm2 start index.js --name "streamaio"
pm2 save
pm2 logs streamaio --lines 10
```

### 7️⃣ **Cek Status Aplikasi**
```bash
pm2 status streamaio
```

### 8️⃣ **Konfigurasi Streaming**
Pastikan Anda sudah memiliki **Stream Key** dari platform streaming yang akan digunakan. Konfigurasinya dapat dilakukan melalui tampilan aplikasi.

---

## 💡 Informasi Tambahan

- Aplikasi ini menggunakan **Express.js** sebagai backend, **SQLite** sebagai database, dan **FFmpeg** untuk encoding serta streaming.
- Antarmuka pengguna dibuat dengan **HTML, CSS, JavaScript**, serta **Tailwind CSS**.
- Aplikasi ini dirancang untuk berjalan di **server dengan Node.js**, bukan di browser lokal.

---

## 🤝 Kontribusi

Jika ingin berkontribusi atau melaporkan bug, silakan buat **Pull Request** atau buka **Issue** di repositori GitHub Anda.

---

## 📜 Lisensi

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/GITHUB_URL_ANDA/streamaio/blob/main/LICENSE)

Hak Cipta © 2025 - [Nama Anda](https://github.com/Twentytwoaio)
