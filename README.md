# Website Portofolio & CV - M. Rafli Parindang

Website personal modern dengan gaya **Creative / Bold**, dibangun menggunakan **HTML5, Modern CSS, dan JavaScript murni**.

## 🚀 Fitur Utama
1. **Hero & Passion Section**: Headline bold, ringkasan profil, dan kartu passion (Web Dev, UI/UX, dll).
2. **Filterable Portfolio**: Galeri proyek kerjaan dengan tombol filter kategori dinamis (*Web App*, *UI/UX*, *Passion Project*).
3. **Halaman CV Interaktif (`cv.html`)**:
   - Timeline pengalaman kerja & proyek.
   - Matriks keahlian (Frontend, Design, Tools, Soft Skills).
   - Riwayat pendidikan & sertifikasi.
   - **Fitur Cetak / Simpan PDF**: Tombol otomatis memicu print browser dengan format kertas A4 putih bersih tanpa navbar (`@media print`).
4. **Responsif & Ringan**: Langsung jalan di browser tanpa perlu `npm install` atau build tool.

## 📁 Struktur File
```text
Web I/
├── index.html            # Halaman utama portofolio & passion
├── cv.html               # Halaman CV interaktif lengkap
├── assets/
│   ├── css/
│   │   └── style.css     # Style utama + cetak PDF (@media print)
│   ├── js/
│   │   └── main.js       # Filter proyek, print CV, navigasi mobile
│   ├── img/              # Letakkan foto profil dan screenshot proyek
│   └── docs/             # Letakkan berkas CV PDF fisik (opsional)
└── README.md
```

## 🛠️ Cara Menjalankan & Menyesuaikan

### 1. Membuka di Browser
- Cukup klik ganda (double-click) file `index.html` di File Explorer, atau
- Gunakan ekstensi *Live Server* di VS Code, atau
- Jalankan via terminal:
  ```powershell
  python -m http.server 3000
  ```
  lalu buka `http://localhost:3000`.

### 2. Personalisasi Konten
- **Foto Profil**: Simpan foto ke `assets/img/profile.jpg`, lalu ganti `<svg>...</svg>` di dalam `.avatar-wrapper` pada `index.html` dengan `<img src="assets/img/profile.jpg" alt="Foto Rafli">`.
- **Proyek**: Tambah atau ubah kartu `<div class="project-card" data-category="web">` di `index.html`.
- **Riwayat CV**: Edit data timeline kerja dan pendidikan di `cv.html`.

### 3. Ekspor PDF CV
- Buka `cv.html` di browser.
- Klik tombol **"Cetak / Simpan PDF"**.
- Pada dialog cetak browser, pilih Destination: **Save as PDF** / **Simpan sebagai PDF**.
