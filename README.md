# Financial Management — Paket Logo

<p align="center"><img src="logo/logo-full-512.png" alt="Logo Financial Management" width="320"></p>

Kumpulan berkas logo **Financial Management** dalam berbagai ukuran dan keperluan: logo penuh, ikon saja, tulisan saja, favicon/ikon aplikasi (PWA), dan gambar untuk media sosial. Semua berkas `PNG` memakai latar **transparan** kecuali yang bernama `white-bg`, `apple-touch-icon`, `maskable`, dan folder `social/`.

## Isi paket

| Berkas | Ukuran | Untuk apa |
|---|---|---|
| `logo/logo-full-1024.png`, `-512`, `-256` | 1024 / 512 / 256 px (persegi) | Logo lengkap (ikon + tulisan), latar transparan. Pakai di latar **terang**. |
| `logo/logo-full-white-bg-1024.png` | 1024 px | Logo lengkap di latar putih, untuk dokumen / slide. |
| `logo/logo-icon-1024.png` … `-64` | 1024, 512, 256, 128, 64 px | Ikon saja (tanpa tulisan): header aplikasi, avatar, profil. |
| `logo/logo-wordmark-1200.png`, `-600` | lebar 1200 / 600 px | Tulisan "Financial Management" saja. |
| `favicon/favicon.ico` | 16, 32, 48, 64 px | Ikon tab browser (semua browser). |
| `favicon/favicon-16x16.png`, `-32x32`, `-48x48` | 16 / 32 / 48 px | Favicon PNG. |
| `favicon/apple-touch-icon.png` | 180 px | Ikon layar utama iPhone/iPad (latar putih). |
| `favicon/android-chrome-192x192.png`, `-512x512` | 192 / 512 px | Ikon aplikasi (PWA) di Android. |
| `favicon/maskable-icon-512x512.png` | 512 px | Ikon PWA "maskable" (latar biru penuh, tidak terpotong). |
| `favicon/site.webmanifest` | — | Manifest PWA yang merujuk ikon di atas. |
| `social/github-social-preview-1280x640.png` | 1280×640 | Unggah di **Settings → Social preview** repositori GitHub. |
| `social/og-image-1200x630.png` | 1200×630 | Gambar pratinjau saat tautan dibagikan (Open Graph). |

## Pasang di situs / aplikasi web

Salin folder `favicon/` ke folder situs Anda, lalu tambahkan di `<head>`:

```html
<link rel="icon" href="favicon/favicon.ico" sizes="any">
<link rel="icon" type="image/png" sizes="32x32" href="favicon/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="favicon/favicon-16x16.png">
<link rel="apple-touch-icon" href="favicon/apple-touch-icon.png">
<link rel="manifest" href="favicon/site.webmanifest">
<meta name="theme-color" content="#014498">

<!-- pratinjau saat tautan dibagikan -->
<meta property="og:image" content="https://DOMAIN-ANDA/social/og-image-1200x630.png">
```

Logo di header aplikasi:

```html
<img src="logo/logo-icon-128.png" alt="Financial Management" width="40" height="40">
```

## Warna

Perkiraan warna utama yang diambil dari logo:

| Nama | Hex |
|---|---|
| Biru tua (teks) | `#003075` |
| Biru utama (latar ikon) | `#014498` |
| Biru cerah (grafik) | `#066BD3` |
| Emas (panah & koin) | `#F9AA02` |

## Pedoman singkat

- Pakai logo penuh di **latar terang**. Teksnya biru tua, jadi kurang terbaca di latar gelap.
- Beri ruang kosong di sekeliling logo minimal sekitar 10% dari lebarnya.
- Ukuran terkecil: ikon 16 px, logo penuh lebar 120 px.
- Jangan diregangkan, diputar, atau diganti warnanya.
- Berkas ini berbasis gambar raster (PNG). Untuk cetak ukuran besar (spanduk, baliho), sebaiknya dibuat ulang sebagai vektor (SVG).

## Unggah ke GitHub

1. Buat repositori baru di github.com (mis. `financial-management-logo`).
2. Pilih **Add file → Upload files**, lalu seret seluruh isi folder ini (termasuk folder `logo`, `favicon`, `social`) dan klik **Commit changes**.
3. Atau lewat terminal:

```bash
cd financial-management-logo
git init -b main
git add .
git commit -m "Tambah paket logo Financial Management"
git remote add origin https://github.com/USERNAME/financial-management-logo.git
git push -u origin main
```

4. Di **Settings → General → Social preview**, unggah `social/github-social-preview-1280x640.png`.
