# 🌾 Panduan Menjalankan Website BUMDes Gotong Royong Sejahtera Secara Lokal

Selamat datang! Panduan ini dibuat untuk memudahkan Anda menjalankan website BUMDes di komputer lokal, meskipun latar belakang Anda bukan dari bidang IT. Ikuti langkah-langkah di bawah dengan teliti.

---

## 📋 Daftar Isi

1. [Langkah 1: Install Visual Studio Code](#langkah-1-install-visual-studio-code)
2. [Langkah 2: Install Node.js](#langkah-2-install-nodejs)
3. [Langkah 3: Download Project](#langkah-3-download-project)
4. [Langkah 4: Buka Project di VS Code](#langkah-4-buka-project-di-vs-code)
5. [Langkah 5: Install Dependencies](#langkah-5-install-dependencies)
6. [Langkah 6: Jalankan Website Secara Lokal](#langkah-6-jalankan-website-secara-lokal)
7. [Troubleshooting - Solusi Masalah](#troubleshooting---solusi-masalah)

---

## 🎯 Persyaratan Sistem

Sebelum memulai, pastikan komputer Anda memenuhi:
- **Sistem Operasi**: Windows 10/11, macOS, atau Linux
- **RAM Minimum**: 4 GB
- **Storage**: Minimal 500 MB ruang kosong
- **Koneksi Internet**: Stabil (untuk download file-file)

---

## Langkah 1: Install Visual Studio Code

Visual Studio Code (VS Code) adalah aplikasi teks editor yang akan kita gunakan untuk membuka dan mengedit kode project.

### Cara Install:

1. **Buka browser** (Chrome, Edge, Firefox, dll) dan kunjungi:
   ```
   https://code.visualstudio.com
   ```

2. **Klik tombol "Download"** yang besar di tengah halaman
   - Pilih sesuai sistem operasi Anda (Windows, Mac, atau Linux)

3. **Tunggu file selesai terunduh**, biasanya bernama `VSCodeSetup-x.x.x.exe` (untuk Windows)

4. **Buka file yang sudah diunduh** dengan double-click

5. **Ikuti wizard instalasi**:
   - Klik "I accept the agreement"
   - Klik "Next"
   - Pilih lokasi instalasi (default sudah oke)
   - Klik "Next" sampai selesai
   - Centang "Launch Visual Studio Code"
   - Klik "Finish"

6. **Tunggu VS Code membuka** - Selesai! ✅

---

## Langkah 2: Install Node.js

Node.js adalah runtime JavaScript yang diperlukan untuk menjalankan project React ini.

### Cara Install:

1. **Buka browser** dan kunjungi:
   ```
   https://nodejs.org
   ```

2. **Pilih versi yang tersedia**:
   - Klik tombol **LTS (Long Term Support)** - ini adalah versi yang stabil
   - Jangan pilih "Current"

3. **Klik "Download"** untuk Windows/Mac sesuai sistem Anda

4. **Buka file installer** yang sudah diunduh (misal: `node-v20.x.x-x64.msi`)

5. **Ikuti wizard instalasi Node.js**:
   - Klik "Next"
   - Centang checkbox "Automatically install the necessary tools"
   - Terus klik "Next" hingga selesai
   - Klik "Finish"

6. **Verifikasi instalasi**:
   - Buka Command Prompt atau PowerShell (tekan `Win + R`, ketik `powershell`, tekan Enter)
   - Ketik perintah ini:
     ```
     node --version
     ```
   - Jika muncul versi (misal: `v20.9.0`), berarti berhasil ✅

---

## Langkah 3: Download Project

Project BUMDes sudah tersimpan di GitHub. Ikuti langkah berikut untuk mendownloadnya:

### Opsi A: Download via Git (Recommended)

1. **Buka Command Prompt atau PowerShell**:
   - Tekan `Win + R`
   - Ketik `powershell`
   - Tekan Enter

2. **Navigasi ke folder tempat Anda ingin menyimpan project**:
   ```
   cd C:\Users\YourUsername\Documents
   ```
   *(Sesuaikan dengan username Anda)*

3. **Jalankan perintah ini untuk clone project**:
   ```
   git clone https://github.com/bumdesgrs/bumdes-landing-page.git
   ```

4. **Tunggu hingga selesai** - folder `bumdes-landing-page` akan dibuat otomatis

### Opsi B: Download Manual (Jika Git tidak terpasang)

1. **Buka browser** dan kunjungi:
   ```
   https://github.com/bumdesgrs/bumdes-landing-page
   ```

2. **Klik tombol hijau "Code"** di tengah-atas halaman

3. **Pilih "Download ZIP"**

4. **Tunggu file selesai terunduh**

5. **Extract file ZIP**:
   - Klik kanan pada file ZIP
   - Pilih "Extract All" atau "Ekstrak Semua"
   - Pilih lokasi folder
   - Selesai!

---

## Langkah 4: Buka Project di VS Code

1. **Buka VS Code** (jika belum terbuka)

2. **Klik "File"** di menu atas

3. **Pilih "Open Folder"**

4. **Cari dan pilih folder `bumdes-landing-page`** yang sudah di-download

5. **Klik "Select Folder"**

6. **Tunggu VS Code memproses** - folder project akan tampil di sisi kiri

---

## Langkah 5: Install Dependencies

Dependencies adalah paket-paket yang dibutuhkan project untuk berjalan.

### Cara Install:

1. **Buka Terminal di VS Code**:
   - Tekan `Ctrl + `` (backtick/tanda petik terbalik)
   - Atau klik "Terminal" → "New Terminal" di menu atas

2. **Terminal akan terbuka di bawah layar**

3. **Ketik perintah berikut**:
   ```
   npm install
   ```

4. **Tekan Enter** dan tunggu proses selesai
   - Ini akan memakan waktu 2-5 menit tergantung kecepatan internet
   - Anda akan melihat banyak teks berjalan - ini normal!

5. **Ketika selesai, Anda akan melihat pesan seperti**:
   ```
   added XXX packages in X.XXs
   ```
   - Ini berarti berhasil ✅

---

## Langkah 6: Jalankan Website Secara Lokal

Setelah semua dependencies terpasang, sekarang saatnya menjalankan website.

### Cara Menjalankan:

1. **Pastikan terminal masih terbuka** di VS Code (jika sudah ditutup, buka lagi dengan `Ctrl + ```)

2. **Ketik perintah berikut**:
   ```
   npm run dev
   ```

3. **Tekan Enter**

4. **Tunggu hingga muncul pesan seperti ini**:
   ```
   VITE v5.x.x ready in XXX ms

   ➜  Local:   http://localhost:5173/
   ```

5. **Buka browser Anda** dan kunjungi:
   ```
   http://localhost:5173
   ```

6. **Website BUMDes akan tampil!** 🎉

---

## 📝 Mengedit Konten Website

Jika ingin mengubah konten website:

1. **Buka file yang ingin diubah** di VS Code:
   - Navigasi ke folder `src/pages/landing-page/components/`
   - Contoh: untuk mengubah teks di bagian "Unit Usaha", buka file `BussinessUnitsSection.jsx`

2. **Edit teks atau data** sesuai kebutuhan

3. **Simpan file** (tekan `Ctrl + S`)

4. **Website akan otomatis refresh** di browser - perubahan langsung terlihat!

### File-file Penting untuk Diketahui:

- `src/pages/landing-page/components/BussinessUnitsSection.jsx` - Unit Usaha
- `src/pages/landing-page/components/FAQSection.jsx` - FAQ/Pertanyaan
- `src/pages/landing-page/components/ContactSection.jsx` - Kontak
- `src/pages/landing-page/components/FooterSection.jsx` - Footer

---

## 🛑 Troubleshooting - Solusi Masalah

### Masalah 1: Command `npm` tidak ditemukan

**Solusi:**
- Pastikan Node.js sudah diinstall dengan benar
- Buka Command Prompt baru dan ketik: `node --version`
- Jika muncul versi, restart VS Code
- Jika masih tidak bisa, uninstall dan reinstall Node.js

### Masalah 2: "EACCES: permission denied"

**Solusi (untuk Mac/Linux):**
```
sudo chown -R $(whoami) ~/.npm
```

### Masalah 3: Port 5173 sudah digunakan

**Solusi:**
- Tutup semua VS Code atau aplikasi lain yang menggunakan port tersebut
- Atau jalankan dengan port berbeda:
  ```
  npm run dev -- --port 5174
  ```

### Masalah 4: `npm install` memakan waktu sangat lama

**Solusi:**
- Ini normal untuk pertama kali (bisa 5-10 menit)
- Pastikan koneksi internet stabil
- Jangan tutup terminal sampai selesai

### Masalah 5: Website tidak tampil di http://localhost:5173

**Solusi:**
- Pastikan terminal masih menjalankan `npm run dev`
- Refresh halaman browser (tekan F5)
- Cek apakah ada error di terminal VS Code
- Jika ada error merah, screenshot dan konsultasikan dengan developer

---

## 🎓 Tips Penting

1. **Selalu jalankan `npm run dev`** sebelum membuka browser
2. **Jangan tutup terminal** selama bekerja - terminal menjalankan server lokal
3. **Simpan file** setelah melakukan perubahan (Ctrl + S)
4. **Refresh browser** jika perubahan tidak terlihat (F5)
5. **Jika ada masalah, cek terminal** - biasanya ada pesan error yang membantu

---

## 📞 Butuh Bantuan?

Jika mengalami kesulitan:

1. **Baca kembali langkah-langkah** di atas dengan teliti
2. **Cek pesan error di terminal** - sering ada petunjuk solusi
3. **Screenshot error** dan kirim ke developer project
4. **Hubungi tim IT** yang menangani project ini

---

## 🎉 Selamat!

Anda sudah berhasil menjalankan website BUMDes secara lokal. Sekarang Anda bisa:
- ✅ Melakukan perubahan pada konten
- ✅ Menambah fitur baru
- ✅ Menguji website sebelum di-deploy

Happy coding! 🚀
