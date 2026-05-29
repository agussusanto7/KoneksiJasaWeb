# 🏠 KoneksiJasa

> **Platform marketplace jasa rumah tangga berbasis web yang menghubungkan pelanggan dengan penyedia jasa terpercaya di sekitar mereka.**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![WhatsApp](https://img.shields.io/badge/WhatsApp_Integration-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)

---

## 📋 Daftar Isi

- [Tentang Proyek](#-tentang-proyek)
- [Fitur Utama](#-fitur-utama)
- [Layanan yang Tersedia](#-layanan-yang-tersedia)
- [Mitra Penyedia Jasa](#-mitra-penyedia-jasa)
- [Cara Kerja](#-cara-kerja)
- [Struktur File](#-struktur-file)
- [Teknologi yang Digunakan](#-teknologi-yang-digunakan)
- [Instalasi & Penggunaan](#-instalasi--penggunaan)
- [Konfigurasi WhatsApp](#-konfigurasi-whatsapp)
- [Menambahkan Layanan & Mitra Baru](#-menambahkan-layanan--mitra-baru)
- [Responsivitas](#-responsivitas)
- [Kontak & Dukungan](#-kontak--dukungan)

---

## 🎯 Tentang Proyek

**KoneksiJasa** adalah sebuah platform marketplace berbasis web (single-page application) yang dirancang untuk mempermudah masyarakat menemukan dan memesan jasa rumah tangga yang profesional dan terpercaya. Platform ini bertindak sebagai jembatan antara pelanggan yang membutuhkan layanan dengan para mitra penyedia jasa yang sudah terverifikasi.

Seluruh proses pemesanan dilakukan melalui integrasi langsung dengan **WhatsApp**, sehingga komunikasi antara pelanggan dan penyedia jasa menjadi lebih mudah, cepat, dan personal—tanpa perlu aplikasi tambahan.

### Tujuan Proyek

- Mempermudah masyarakat menemukan jasa rumah tangga berkualitas di sekitar mereka
- Memberikan platform digital bagi penyedia jasa lokal untuk memperluas jangkauan pelanggan
- Menyederhanakan proses pemesanan melalui alur WhatsApp yang sudah familiar bagi kebanyakan pengguna Indonesia

---

## ✨ Fitur Utama

| Fitur | Deskripsi |
|---|---|
| 📱 **Booking via WhatsApp** | Formulir pemesanan yang otomatis mengirim detail order ke WhatsApp admin |
| 🔗 **Direct Chat Mitra** | Tombol chat langsung ke WhatsApp masing-masing mitra penyedia jasa |
| 🎨 **Desain Responsif** | Tampilan optimal di semua ukuran layar (desktop, tablet, mobile) |
| ✅ **Validasi Formulir** | Validasi input real-time dengan pembatasan tanggal minimum (tidak bisa pesan tanggal lampau) |
| 🗓️ **Pemilihan Jadwal** | Pelanggan dapat memilih tanggal dan waktu layanan yang diinginkan |
| 💬 **Floating WhatsApp Button** | Tombol WhatsApp yang selalu terlihat untuk kontak cepat ke admin |
| 🎥 **Animasi Scroll** | Kartu layanan dan mitra muncul dengan animasi saat di-scroll menggunakan Intersection Observer API |
| 🖼️ **Modal Booking** | Pop-up form pemesanan yang bersih tanpa pindah halaman |
| 📜 **Smooth Scrolling** | Navigasi antar section dengan efek scroll yang halus |

---

## 🛠️ Layanan yang Tersedia

### 🌱 Potong Rumput
- Layanan pemotongan rumput profesional untuk halaman rumah
- Tersedia paket reguler (berlangganan) dan *one-time service*
- **Harga mulai:** Rp 80.000

### 🚗 Cuci Mobil
- Cuci mobil premium menggunakan produk berkualitas
- Meliputi cuci eksterior, pembersihan interior, dan *waxing*
- **Harga mulai:** Rp 100.000

### ❄️ Service AC
- Jasa service dan perawatan AC untuk rumah maupun kantor
- Mencakup *cleaning*, isi freon, dan perbaikan unit
- **Harga mulai:** Rp 120.000

---

## 👥 Mitra Penyedia Jasa

| Nama Mitra | Spesialisasi | Rating | Nomor WhatsApp |
|---|---|---|---|
| **Erwin Gardening** | Potong rumput & perawatan taman | ⭐ 4.9 | 081237575743 |
| **Firman Car Wash** | Cuci mobil premium | ⭐ 4.8 | 085812882170 |
| **Erlangga Green Care** | Perawatan tanaman & landscaping | ⭐ 4.9 | 082269502453 |
| **Kelvin Multi Service** | Cuci motor, poles mobil, maintenance kendaraan | ⭐ 4.7 | 082233665564 |
| **Agus AC Service** | Service & perbaikan semua merk AC | ⭐ 4.8 | 085785672280 |

---

## ⚙️ Cara Kerja

Berikut adalah alur penggunaan platform KoneksiJasa dari sisi pelanggan:

```
1. Pelanggan membuka website KoneksiJasa
         │
         ▼
2. Memilih layanan yang dibutuhkan (Potong Rumput / Cuci Mobil / Service AC)
         │
         ├─── Opsi A: Klik "Pesan Layanan" → Isi form booking → Kirim ke WhatsApp Admin
         │
         └─── Opsi B: Klik "Chat [Nama Mitra]" → Langsung ke WhatsApp Mitra Terkait
         │
         ▼
3. Admin/Mitra menerima pesan WhatsApp berisi detail pesanan
         │
         ▼
4. Admin/Mitra mengkonfirmasi jadwal dan detail kepada pelanggan
         │
         ▼
5. Layanan dilaksanakan sesuai jadwal yang disepakati
```

### Format Pesan WhatsApp Otomatis

Ketika pelanggan mengisi dan mengirim form booking, sistem akan otomatis membuat pesan terformat seperti berikut dan membukanya di WhatsApp:

```
🏠 *PESANAN BARU KONEKSIJASA* 🏠

📋 *Detail Pesanan:*
• Layanan: Cuci Mobil
• Nama: Budi Santoso
• WhatsApp: 08123456789
• Alamat: Jl. Mawar No. 10, Malang
• Tanggal: Senin, 2 Juni 2025
• Waktu: 09:00
• Catatan: Mobil SUV, tolong poles juga

Mohon konfirmasi ketersediaan jadwal. Terima kasih! 🙏
```

---

## 📁 Struktur File

Proyek ini merupakan aplikasi single-page sederhana yang terdiri dari satu file utama:

```
koneksijasa/
│
└── index.html          # File utama (HTML + CSS + JavaScript dalam satu file)
```

Seluruh kode — struktur HTML, styling CSS, dan logika JavaScript — dikemas dalam satu file `index.html` untuk kemudahan deployment dan distribusi.

---

## 🔧 Teknologi yang Digunakan

- **HTML5** — Struktur dan semantik halaman web
- **CSS3** — Styling, animasi, dan layout responsif
  - CSS Grid & Flexbox untuk tata letak
  - CSS Animations & Transitions untuk efek visual
  - `backdrop-filter` untuk efek kaca buram pada header
  - Media Queries untuk responsivitas
- **Vanilla JavaScript (ES6+)** — Logika interaktif tanpa framework tambahan
  - `Intersection Observer API` untuk animasi scroll
  - `window.open()` untuk membuka WhatsApp di tab baru
  - `encodeURIComponent()` untuk encoding pesan WhatsApp
  - Event Listeners untuk interaksi pengguna
- **WhatsApp Business API** — Integrasi pemesanan via `wa.me` deeplink

---

## 🚀 Instalasi & Penggunaan

Karena ini adalah proyek static HTML murni, **tidak diperlukan instalasi, build process, atau server khusus**.

### Cara Menjalankan Secara Lokal

1. **Clone atau unduh** file `index.html` ke komputer Anda
2. **Buka file** `index.html` langsung di browser (double-click), atau
3. **Gunakan Live Server** jika menggunakan VS Code untuk pengalaman development yang lebih baik:
   - Install ekstensi **Live Server** di VS Code
   - Klik kanan pada `index.html` → **Open with Live Server**

### Deployment

Website ini dapat di-deploy ke platform hosting statis mana pun:

- **[GitHub Pages](https://pages.github.com/)** — Gratis, push ke repo GitHub dan aktifkan Pages
- **[Netlify](https://netlify.com)** — Drag & drop folder ke dashboard Netlify
- **[Vercel](https://vercel.com)** — Import dari GitHub atau upload langsung
- **Shared Hosting** — Upload `index.html` ke direktori `public_html` via FTP/cPanel

---

## 📲 Konfigurasi WhatsApp

Semua nomor WhatsApp dikonfigurasi langsung di dalam file `index.html`. Untuk mengubah nomor, cari dan ganti nilai berikut:

### Nomor Admin Utama (untuk terima semua booking)

Cari teks berikut di file `index.html` dan ganti nomornya:

```html
<!-- WhatsApp Float Button -->
<a href="https://wa.me/62895383015559?text=..." ...>

<!-- Pada form submission di JavaScript -->
const waUrl = `https://wa.me/62895383015559?text=...`;

<!-- Footer -->
<p>... WhatsApp: 0895383015559</p>
```

### Nomor Masing-Masing Mitra

Setiap mitra memiliki tombol chat langsung. Format URL WhatsApp-nya:

```
https://wa.me/[kode_negara][nomor_tanpa_0]?text=[pesan_awal_terenkode]
```

Contoh untuk nomor `081237575743`:
```
https://wa.me/6281237575743?text=Halo%20Erwin%2C%20saya%20ingin%20memesan...
```

> **Catatan:** Kode negara Indonesia adalah `62`. Hilangkan angka `0` di awal nomor saat menulis URL WhatsApp (contoh: `081xxx` → `6281xxx`).

---

## ➕ Menambahkan Layanan & Mitra Baru

### Menambahkan Kartu Layanan Baru

Tambahkan blok berikut di dalam `<div class="services-grid">` pada file `index.html`:

```html
<div class="service-card">
    <div class="service-icon">🔧</div>  <!-- Ganti dengan emoji yang sesuai -->
    <h3>Nama Layanan</h3>
    <p>Deskripsi singkat tentang layanan ini.</p>
    <div class="price">Mulai dari Rp XX.000</div>
    <button class="contact-btn" onclick="openBookingModal('Nama Layanan')">Pesan Layanan</button>
</div>
```

### Menambahkan Kartu Mitra Baru

Tambahkan blok berikut di dalam `<div class="providers-grid">`:

```html
<div class="provider-card">
    <div class="provider-avatar">👨</div>  <!-- atau 👩 -->
    <h3>Nama Mitra</h3>
    <div class="rating">⭐⭐⭐⭐⭐ (4.x)</div>
    <p>Deskripsi singkat keahlian mitra.</p>
    <a href="https://wa.me/628XXXXXXXXXX?text=Halo%20[Nama]%2C%20saya%20ingin%20memesan%20jasa"
       class="contact-btn"
       target="_blank">Chat [Nama]</a>
</div>
```

---

## 📱 Responsivitas

Website dirancang responsif menggunakan CSS Grid dengan `auto-fit` dan `minmax`, serta Media Query untuk layar kecil:

| Ukuran Layar | Tampilan |
|---|---|
| **Desktop** (> 768px) | 3 kolom untuk layanan, grid mitra multi-kolom, navigasi penuh |
| **Mobile** (≤ 768px) | 1 kolom untuk semua kartu, navigasi disembunyikan, layout stack vertikal |

---

## 📞 Kontak & Dukungan

Untuk pertanyaan teknis, penambahan fitur, atau kerjasama:

- **WhatsApp Admin:** [0895383015559](https://wa.me/62895383015559)
- **Platform:** KoneksiJasa

---

## 📄 Lisensi

© 2025 KoneksiJasa. Semua hak dilindungi.

---

<div align="center">
  <sub>Dibuat dengan ❤️ untuk membantu UMKM jasa lokal berkembang secara digital</sub>
</div>
