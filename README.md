# 🎓 **SIEGA – UNIKA Soegijapranata**
Website Informasi Program Studi  
Sistem Informasi · E-Commerce · Game Teknologi · Akuntansi Sistem Informasi

---

## 📘 **Tentang Proyek**
Proyek ini adalah sebuah website landing page untuk memperkenalkan empat program studi di bawah kelompok **SIEGA** (Sistem Informasi, E-Commerce, Game Teknologi, dan Akuntansi Sistem Informasi) Universitas Katolik Soegijapranata.

Website ini dibuat menggunakan **HTML**, **CSS**, dan **JavaScript**. Seluruh konten pada halaman seperti program studi, kurikulum, profil, keunggulan, dan kontak diambil langsung dari file `index.html` dan `siega.js` yang kamu berikan.

---

## ✨ **Fitur-Fitur Utama (Sesuai Kode Asli)**

### 🔹 **1. Navbar dengan Smooth Scroll**
- Navbar fixed di bagian atas  
- Efek mengecil saat halaman di-scroll  
- Smooth scroll untuk navigasi  
- Dibangun dari struktur `<nav>` dalam `index.html`

### 🔹 **2. Hero Section**
- Background gradient gelap  
- Efek lingkaran glow animasi (`@keyframes pulse` dalam `style.css`)  
- Teks animasi fade-in (`fadeInUp`)  
- Tombol CTA:  
  - “Lihat Program SIEGA”  
  - “Daftar Sekarang”

### 🔹 **3. Programs Section**
Bagian ini menampilkan **4 program studi**, sesuai isi `index.html`:

1. 💻 Sistem Informasi  
2. 🛒 E-Commerce  
3. 🎮 Game Teknologi  
4. 📊 AKSI (Akuntansi Sistem Informasi)

Setiap card memiliki:  
- Ikon emoji  
- Deskripsi singkat  
- List kompetensi  
- Tombol **Lihat Kurikulum**

### 🔹 **4. Kurikulum Dinamis (Data dari `siega.js`)**
Data kurikulum **bukan hardcoded di HTML**, tapi diambil dari:

```js
const curriculumData = {
    SI: {...},
    EC: {...},
    GT: {...},
    AKSI: {...}
}
```

Fitur kurikulum:
- Ditampilkan berdasarkan program yang klik tombolnya  
- Tabel berisi:  
  - Mata Kuliah  
  - SKS  
  - Capaian Pembelajaran  
- Tombol **“Download PDF Kurikulum”** (simulasi, memunculkan alert)
- Default saat halaman dibuka: `showCurriculum('SI')`

### 🔹 **5. Profil SIEGA**
Teks lengkap sesuai `index.html`, termasuk:
- Penjelasan tentang SIEGA  
- Visi  
- Misi  
- Nilai-nilai UNIKA (Integritas, Profesionalitas, Humanisme)  
- Keunggulan SIEGA (✨ Dosen profesional dll.)

### 🔹 **6. Contact Section**
Data kontak sesuai file:
- Email: **siega@unika.ac.id**  
- WhatsApp: **+62 812-3456-7890**  
- Alamat kampus  
- Social button: Instagram, Website, Facebook  
- Tombol **Daftar Sekarang**

### 🔹 **7. Animasi Scroll**
Di-handle menggunakan `IntersectionObserver`:

```js
section.style.opacity = '0';
section.style.transform = 'translateY(30px)';
```

Saat terlihat, berubah menjadi:
- opacity 1
- translateY(0)  

### 🔹 **8. Responsive Design (dari `style.css`)**
Pada breakpoint max-width: 768px:
- Font Hero mengecil  
- CTA berubah vertikal  
- Grid mengecil  
- Navbar menyembunyikan nav-links  

---

## 📁 **Struktur File (Sesuai yang Kamu Upload)**
```
📂 project-folder
│── index.html       → Struktur halaman & konten utama
│── style.css        → Styling, layout, animasi, responsive
│── siega.js         → Data kurikulum + script interaktif
└── README.md        → Dokumentasi proyek
```

---

## 🛠️ **Teknologi yang Digunakan**
- **HTML5**  
- **CSS3** (gradient, shadow, animasi, responsive)  
- **JavaScript (Vanilla)**  
  - DOM Manipulation  
  - Smooth Scroll  
  - Dynamic Content Rendering  
  - Intersection Observer  

---

## 🚀 **Cara Menjalankan**
1. Download atau clone repository:
   ```bash
   git clone https://github.com/username/repo.git
   ```
2. Pastikan file berikut berada dalam satu folder:
   - index.html  
   - style.css  
   - siega.js  
3. Buka file:
   ```
   index.html
   ```
4. Website berjalan secara lokal di browser.

Tidak memerlukan server.

---

## 📝 **Pengembangan Selanjutnya (Opsional)**
(Saran berdasarkan struktur file kamu)

- Tambah fitur **download PDF yang asli**, bukan alert  
- Tambah halaman detail program  
- Tambah halaman login untuk admin input kurikulum  
- Tambah dark mode dengan CSS variables  
- Hosting ke GitHub Pages  

---

## 📄 **Lisensi**
Website ini dibuat untuk tujuan edukasi.  
Pengguna diperbolehkan mengubah, mengembangkan, dan menggunakan kembali proyek ini.

