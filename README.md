<div align="center">

# 🚀 Landing Page Google Ads Project

### Landing page berkonversi tinggi, ringan, dan siap dipasang untuk kampanye Google Ads

<br />

`HTML5` &nbsp;•&nbsp; `CSS3` &nbsp;•&nbsp; `JavaScript` &nbsp;•&nbsp; `Google Ads`

`Status: Aktif` &nbsp;•&nbsp; `Responsif` &nbsp;•&nbsp; `Lisensi: MIT` &nbsp;•&nbsp; `Made in Indonesia 🇮🇩`

<br />

[✨ Fitur](#-fitur-utama) •
[🧰 Tech Stack](#-tech-stack) •
[📁 Struktur](#-struktur-folder) •
[⚡ Instalasi](#-instalasi--menjalankan) •
[🎯 Integrasi Ads](#-integrasi-google-ads) •
[🛠️ Kustomisasi](#️-kustomisasi)

</div>

---

## 📖 Tentang Proyek

**Landing Page Google Ads Project** adalah koleksi halaman landing yang dirancang khusus untuk kebutuhan **iklan Google Ads**. Fokus utamanya: **kecepatan muat**, **pesan yang jelas**, dan **CTA yang mudah dikonversi** — tiga hal yang sangat memengaruhi *Quality Score* dan biaya per konversi.

Dibangun murni dengan **HTML, CSS, dan JavaScript** tanpa framework berat, sehingga mudah dipahami, cepat dimuat, dan bisa di-hosting di mana saja (hosting biasa, GitHub Pages, Netlify, Vercel, dll).

> 💡 Bagian dari repository **Kumpulan Project Saya**.

---

## ✨ Fitur Utama

| | Fitur | Keterangan |
|---|---|---|
| ⚡ | **Super Ringan** | Tanpa dependensi berat, skor PageSpeed tinggi |
| 📱 | **Mobile First** | Tampilan responsif di semua ukuran layar |
| 🎯 | **CTA Jelas** | Tombol aksi menonjol: WhatsApp, form, atau telepon |
| 🧲 | **Struktur Konversi** | Hero → Manfaat → Bukti sosial → Penawaran → CTA |
| 📊 | **Siap Tracking** | Slot untuk Google Tag, GA4, dan konversi Google Ads |
| 🎬 | **Animasi Halus** | Scroll reveal & hover effect dengan JavaScript ringan |
| 🔍 | **SEO Dasar** | Meta tag, heading terstruktur, dan atribut alt |
| 🧩 | **Mudah Dikustomisasi** | Warna & teks diatur lewat CSS variables |

---

## 🧰 Tech Stack

| Teknologi | Peran |
|:---|:---|
| 🟧 **HTML5** | Struktur & semantik halaman |
| 🟦 **CSS3** | Layout (Flexbox/Grid), styling, animasi, responsif |
| 🟨 **JavaScript** | Interaksi, validasi form, scroll effect, tracking event |

---

## 📁 Struktur Folder

```bash
landing-page-google-ads/
├── 📄 index.html          # Halaman utama landing page
├── 📂 assets/
│   ├── 📂 css/
│   │   └── style.css      # Seluruh styling & variabel warna
│   └── 📂 js/
│       └── main.js        # Interaksi, form, & event tracking
├── 📄 README.md
└── 📄 LICENSE
```

> 📌 Sesuaikan struktur di atas dengan susunan folder aktual di repository kamu.

---

## ⚡ Instalasi & Menjalankan

### 1️⃣ Clone repository

```bash
git clone https://github.com/USERNAME/NAMA-REPO.git
cd NAMA-REPO/landing-page-google-ads
```

### 2️⃣ Jalankan secara lokal

Cukup buka `index.html` di browser, atau gunakan live server:

```bash
# Opsi 1 — Python
python -m http.server 8000

# Opsi 2 — Node.js
npx serve .
```

Lalu buka **http://localhost:8000** di browser.

### 3️⃣ Deploy

Upload folder ke hosting favoritmu:

- 🌐 **Hosting / cPanel** — upload via File Manager
- 🐙 **GitHub Pages** — aktifkan di *Settings → Pages*
- ▲ **Vercel / Netlify** — hubungkan repository, deploy otomatis

---

## 🎯 Integrasi Google Ads

### Pasang Google Tag

Letakkan di dalam `<head>` pada `index.html`:

```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=AW-XXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'AW-XXXXXXXXX');
</script>
```

### Lacak Konversi (klik tombol / submit form)

```javascript
function trackConversion() {
  gtag('event', 'conversion', {
    'send_to': 'AW-XXXXXXXXX/YYYYYYYYYYYY'
  });
}

document.querySelectorAll('[data-track="cta"]').forEach((btn) => {
  btn.addEventListener('click', trackConversion);
});
```

> Ganti `AW-XXXXXXXXX` dan `YYYYYYYYYYYY` dengan **Conversion ID** dan **Conversion Label** dari akun Google Ads kamu.

---

## 🛠️ Kustomisasi

Ubah tampilan cukup lewat **CSS variables** di `style.css`:

```css
:root {
  --primary: #2563eb;     /* warna utama */
  --accent: #f59e0b;      /* warna tombol CTA */
  --bg: #ffffff;          /* latar belakang */
  --text: #0f172a;        /* warna teks */
  --radius: 14px;         /* kelengkungan sudut */
}
```

Ganti nomor WhatsApp pada tombol CTA:

```html
<a href="https://wa.me/62XXXXXXXXXXX?text=Halo,%20saya%20tertarik"
   class="btn btn-cta" data-track="cta">
  Hubungi Kami
</a>
```

---

## ✅ Checklist Sebelum Tayang

- [ ] Judul & headline sesuai dengan **kata kunci** dan teks iklan
- [ ] Google Tag & **konversi** sudah terpasang dan diuji
- [ ] Gambar sudah dikompres (format WebP bila memungkinkan)
- [ ] Tampilan mobile sudah dicek di beberapa perangkat
- [ ] Skor **PageSpeed Insights** di atas 90
- [ ] Kebijakan privasi & kontak tersedia
- [ ] Semua tombol CTA berfungsi dengan benar

---

## 🗺️ Roadmap

- [ ] Template landing page multi-niche
- [ ] Dukungan A/B testing sederhana
- [ ] Mode gelap (dark mode)
- [ ] Integrasi form ke Google Sheets / WhatsApp API
- [ ] Optimasi gambar otomatis

---

## 🤝 Kontribusi

Saran dan perbaikan sangat diterima!

1. Fork repository ini
2. Buat branch baru: `git checkout -b fitur/nama-fitur`
3. Commit perubahan: `git commit -m "Tambah fitur ..."`
4. Push ke branch: `git push origin fitur/nama-fitur`
5. Buka **Pull Request**

---

## 📄 Lisensi

Didistribusikan di bawah lisensi **MIT**. Lihat berkas `LICENSE` untuk informasi lebih lanjut.

---

<div align="center">

### 👨‍💻 Dibuat oleh **Muhammad Setyo Wibowo**

SEO Content Writer • Digital Content Specialist • Web Developer

🌐 [SenaThreads.id](https://senathreads.id) &nbsp;•&nbsp; 🐙 [GitHub](https://github.com/USERNAME)

<br />

⭐ **Jika proyek ini bermanfaat, jangan lupa beri bintang!** ⭐

</div>
