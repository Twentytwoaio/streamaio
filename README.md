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

## 📌 Catatan

> **Sebelum memulai**, pastikan Anda telah mengunggah kode StreamAio ini ke repositori GitHub Anda sendiri.  
> Jika belum, ikuti langkah-langkah berikut:

### **⚠️ Upload Kode ke GitHub**
Jika belum memiliki repositori GitHub, buat dan unggah kode dengan perintah berikut:

```bash
# Inisialisasi Git dan buat repositori baru
git init
git remote add origin https://github.com/GITHUB_USERNAME_ANDA/streamaio.git
git add .
git commit -m "Inisialisasi proyek StreamAio"
git branch -M main
git push -u origin main
```

## 📌 Cara Instalasi

> **Sebelum mulai:** Pastikan server / VPS kamu sudah terinstall Node.js, npm, dan FFmpeg sebelum meng-clone repositori ini.

### 1️⃣ **Install Node.js dan npm melalui NodeSource PPA:**
```bash
curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
sudo apt-get install -y nodejs
sudo apt-get install -y npm
```
Cek apakah instalasi berhasil:
```bash
node -v
npm -v
```

### 2️⃣ **Install FFmpeg**
```bash
sudo apt-get update
sudo apt-get install -y ffmpeg
```
Cek apakah instalasi berhasil:
```bash
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
Kembali ke directory root (jika masih di directory streamaio)
```bash
cd ..
```

🚀 Perintah menjalankan aplikasi ✨
```bash
pm2 start streamaio
pm2 logs streamaio -i 0 --lines 1
```

📈 Melihat status aplikasi berjalan
```bash
pm2 status streamaio
```

⛔ Menghentikan aplikasi
```bash
pm2 stop streamaio
```

### 7️⃣ **Konfigurasi Streaming**
* Pastikan kamu sudah mengatur URL RTMP yang sesuai untuk setiap platform yang ingin digunakan. Konfigurasi ini bisa dilakukan langsung melalui tampilan aplikasi.
* Silahkan dapatkan Stream Key dari platform streaming yang kamu gunakan.

---

## 💡 Informasi Tambahan

- Aplikasi ini menggunakan **Express.js** sebagai backend, **SQLite** sebagai database, dan **FFmpeg** untuk encoding serta streaming.
- Antarmuka pengguna dibuat dengan **HTML, CSS, JavaScript**, serta **Tailwind CSS**.
- Aplikasi ini dirancang untuk berjalan di **server dengan Node.js**, bukan di browser lokal.

---

## 📜 Lisensi

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/Twentytwoaio/streamaio/blob/main/LICENSE)

Hak Cipta © 2025 - [Twentytwo Aio](https://github.com/Twentytwoaio)
