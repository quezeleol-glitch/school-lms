# School LMS - Mobile & Web App

Aplikasi Learning Management System (LMS) berbasis web dan Android (APK) yang dikembangkan dengan HTML/JS dan dibundel menggunakan Capacitor & GitHub Actions.

---

## 📁 Struktur Proyek

```text
school-lms/
├── .github/
│   └── workflows/
│       └── build-apk.yml    # Workflow GitHub Actions untuk build APK otomatis
├── www/
│   ├── index.html           # File HTML utama
│   └── app.js               # Logika frontend JavaScript (School Lms.js)
├── index.html               # Entry point versi web
├── app.js                   # Logika frontend JavaScript
└── README.md                # Dokumentasi proyek
```

---

## 🚀 Cara Menjalankan Versi Web

### 1. Menjalankan secara Lokal
1. Ekstrak file zip ini ke folder komputer Anda.
2. Buka file `index.html` langsung di browser favorit Anda (Chrome, Firefox, Edge, dll.).

### 2. Deploy ke GitHub Pages / Vercel
* **GitHub Pages:**
  1. Upload seluruh file proyek ke repositori GitHub Anda.
  2. Buka **Settings** -> **Pages**.
  3. Pilih branch `main` / `master` dan folder `/ (root)`, lalu klik **Save**.
* **Vercel / Netlify:**
  1. Hubungkan repositori GitHub Anda ke Vercel/Netlify.
  2. Klik **Deploy** (secara otomatis Vercel mendeteksi `index.html`).

---

## 📱 Cara Membuat APK Android Otomatis (GitHub Actions)

Proyek ini telah dilengkapi dengan workflow GitHub Actions (`.github/workflows/build-apk.yml`) untuk membuat file `.apk` Android secara otomatis:

1. **Push proyek ke GitHub:**
   Upload folder ini ke repositori GitHub Anda (pastikan folder `.github/workflows/build-apk.yml` ikut ter-upload).
2. **Jalankan Workflow:**
   * Buka tab **Actions** di repositori GitHub Anda.
   * Pilih workflow **Build Android APK**.
   * Klik **Run workflow**.
3. **Unduh APK:**
   Setelah proses *build* selesai (sekitar 2–4 menit), klik hasil *run* terbaru, lalu unduh file APK dari bagian **Artifacts** (`app-release.apk`).

---

## 🛠️ Modifikasi & Pengembangan
* Untuk mengedit tampilan/struktur HTML, sesuaikan file `index.html`.
* Untuk memperbarui logika aplikasi, perbarui file `app.js`.
