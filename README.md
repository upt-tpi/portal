# 🛳️ Portal Aplikasi UPT-TPI

Aplikasi portal berbasis HTML/CSS/JS untuk mengelola dan mengakses berbagai aplikasi UPT Tempat Pelelangan Ikan (TPI). Dilengkapi dengan sistem login modern dan integrasi Google Spreadsheet sebagai backend.

---

## 📁 Struktur File

```
portal-tpi/
├── index.html      # Halaman login (entry point)
├── portal.html     # Halaman portal aplikasi (dilindungi login)
├── README.md       # Dokumentasi ini
└── .nojekyll       # Menonaktifkan Jekyll (opsional)
```

---

## 🚀 Cara Deploy ke GitHub Pages

### Langkah 1: Buat Repository GitHub

1. Buka [github.com](https://github.com) dan login
2. Klik tombol **+** (New repository)
3. Beri nama repository: `portal-tpi` (atau nama lain)
4. Pilih **Public** (wajib untuk GitHub Pages gratis)
5. Klik **Create repository**

### Langkah 2: Upload File

**Opsi A: Via Web (Tanpa Git)**

1. Di halaman repository, klik **Add file → Upload files**
2. Upload `index.html` dan `portal.html`
3. Klik **Commit changes**

**Opsi B: Via Git (Command Line)**

```bash
# Clone repository (ganti USERNAME dengan username GitHub Anda)
git clone https://github.com/USERNAME/portal-tpi.git
cd portal-tpi

# Copy file ke folder ini
cp /path/to/index.html .
cp /path/to/portal.html .

# Push ke GitHub
git add .
git commit -m "Initial commit: Portal TPI"
git push origin main
```

### Langkah 3: Aktifkan GitHub Pages

1. Di repository, klik tab **Settings**
2. Di sidebar kiri, klik **Pages**
3. Di bagian **Build and deployment**:
   - Source: pilih **Deploy from a branch**
   - Branch: pilih **main** (atau master)
   - Folder: pilih **/(root)**
4. Klik **Save**

### Langkah 4: Akses Website

Tunggu 1-2 menit, lalu akses:

```
https://USERNAME.github.io/portal-tpi/
```

Ganti `USERNAME` dengan username GitHub Anda.

---

## 🔐 Login Demo

| Field | Nilai |
|-------|-------|
| Username | `admin` |
| Password | `admin123` |

> ⚠️ **Penting:** Ganti kredensial demo dengan validasi API backend Anda sebelum digunakan di produksi.

---

## ⚙️ Konfigurasi Backend (Google Apps Script)

1. Buka Google Spreadsheet → **Extensions → Apps Script**
2. Paste kode backend (Code.gs) yang sudah disediakan
3. Jalankan fungsi `initDefaultData` (satu kali saja)
4. Deploy sebagai **Web App**:
   - Execute as: **Me**
   - Who can access: **Anyone**
5. Salin URL Web App
6. Buka aplikasi → klik **⚙ Konfigurasi** → paste URL di tab **API Backend**

---

## 🎨 Fitur

- ✅ Login page dengan animasi modern (glassmorphism + animated orbs)
- ✅ Session management via localStorage
- ✅ Logout dengan konfirmasi
- ✅ Dark theme konsisten
- ✅ Responsive design
- ✅ Integrasi Google Spreadsheet
- ✅ CRUD aplikasi
- ✅ Test koneksi API

---

## 📧 Kontak

Dikembangkan oleh **Doni Yan Ariyanto / Rumah Koding Rembang**

Email: [doni.yan27@gmail.com](mailto:doni.yan27@gmail.com)

---

## 📄 Lisensi

Proyek ini gratis untuk digunakan dan dimodifikasi.
