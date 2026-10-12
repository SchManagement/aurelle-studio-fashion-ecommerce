# AURELLE STUDIO — Premium Fashion E-Commerce

Website fashion e-commerce statis untuk brand fiktif **AURELLE STUDIO**.

## Teknologi

Project ini dibuat hanya menggunakan:

- HTML5
- CSS3
- Vanilla JavaScript

Tanpa:

- React
- Vue
- Angular
- TypeScript
- Tailwind
- Bootstrap
- jQuery
- Build process

## Struktur File

```text
fashion-ecommerce/
├── index.html
├── style.css
├── app.js
├── README.md
└── assets/
    ├── icons/
    └── images/
        ├── products/
        ├── banners/
        ├── lifestyle/
        └── logo/
```

## Cara Menjalankan

Bisa langsung dibuka lewat browser:

```text
index.html
```

Atau gunakan static server sederhana:

```bash
python -m http.server 8000
```

Lalu buka:

```text
http://localhost:8000
```

## Fitur Utama

- Announcement bar
- Sticky navbar
- Mobile menu
- Hero campaign section
- Featured collection cards
- Product grid
- Search panel
- Filter & sorting
- Quick view modal
- Wishlist berbasis `localStorage`
- Cart drawer berbasis `localStorage`
- Best seller section
- Brand story
- Promo banner
- Trust section
- Testimonials
- Lookbook grid
- Newsletter
- FAQ accordion
- Footer lengkap

## Data Produk

Semua data produk berada di file `app.js` dalam array:

```js
const products = [...]
```

Di sana Anda bisa mengubah:

- nama produk
- kategori
- harga
- deskripsi
- ukuran
- warna
- gambar
- badge
- rating

## Aset Gambar

Gambar produk, hero, dan lifestyle sudah disiapkan di:

```text
assets/images/products/
assets/images/banners/
assets/images/lifestyle/
```

## Ikon Lokal

Semua ikon SVG lokal ada di:

```text
assets/icons/
```

Tidak ada dependensi icon CDN.

## Menyesuaikan Kontak

Informasi kontak footer bisa diubah langsung di `index.html`.

## Deployment

Website ini siap dideploy ke:

- Vercel
- Netlify
- GitHub Pages
- Shared hosting statis

Tidak membutuhkan proses build.

## Catatan

Karena ini adalah website statis:
- checkout masih berupa simulasi
- data cart/wishlist tersimpan lokal di browser
- tidak ada backend pembayaran nyata

Jika Anda mau, project ini bisa dilanjutkan ke versi:
- multi page
- backend PHP / Node.js
- integrasi database
- checkout real
- admin dashboard
- autentikasi user

## Aset Gambar Final

Versi final ini sudah menggunakan 10 gambar katalog/campaign yang diberikan untuk AURELLE STUDIO.

Mapping utama:

- `baju1.png` → Celeste Satin Dress
- `baju2.png` → Luna Oversized Shirt
- `baju3.png` → Amara Pleated Skirt
- `baju4.png` → Elora Knit Cardigan
- `baju5.png` → Aurelle Linen Blouse
- `baju6.png` → Lookbook editorial
- `baju7.png` → Hero campaign
- `baju8.png` → Sofia Basic Top
- `baju9.png` → Nara Premium Set
- `baju10.png` → Aruna Wide Leg Pants

Semua gambar sudah dikonversi menjadi WebP untuk penggunaan web yang lebih efisien.



## V2 Complete — Penyempurnaan

Versi ini melengkapi detail yang sebelumnya belum penuh:

- Typography menggunakan **Playfair Display** dan **Inter** melalui Google Fonts.
- Struktur koleksi lengkap:
  - Dress Collection: Satin Dress, Midi Dress, Casual Dress
  - Tops Collection: Blouse, Shirt, Basic Top
  - Bottom Collection: Pants, Skirt
  - Outer Collection: Cardigan, Jacket, Outerwear
  - Complete Outfit: Matching Set, Casual Set
- Quick View memiliki **3 gambar gallery per produk** yang berasal dari gambar final pengguna.
- Tombol Account sekarang memiliki profil lokal yang tersimpan di `localStorage`.
- Checkout memiliki alur:
  1. Data & alamat pengiriman
  2. Pilihan metode pembayaran demo
  3. Review pesanan
  4. Nomor pesanan & konfirmasi
- Data order demo disimpan lokal pada browser.
- Checkout tidak memproses pembayaran finansial nyata karena project ini statis tanpa backend/payment gateway.


## V3 Fixed — Startup Bug & UI Alignment

Perbaikan utama:

- Menambahkan rule global `[hidden] { display: none !important; }`.
- Cart drawer, search, wishlist, account, Quick View, dan Checkout sekarang dipastikan tertutup saat halaman pertama dibuka.
- JavaScript menjalankan `resetInitialUI()` ketika website dimuat.
- Alignment navbar diperbaiki pada desktop 993–1180px.
- Heading menggunakan balanced wrapping agar baris terlihat lebih editorial.
- Category card dibuat sama tinggi dan CTA tetap sejajar.
- Nama produk, kategori, harga, dan rating dirapikan agar konsisten antar card.
- Layout checkout, quick view, testimonial, footer, dan mobile typography diperhalus.


## V4 — Hero Floating Cards & Wishlist Icon

Perbaikan:

- Floating card **NEW COLLECTION** dipindahkan ke sisi kiri atas area kosong hero image agar tidak menutupi wajah model.
- Floating card **Gratis Ongkir** diposisikan konsisten di dalam frame hero.
- Hero image sekarang menggunakan frame penuh sehingga floating card tidak terlihat keluar dari komposisi.
- Icon wishlist/heart diganti menjadi SVG line heart simetris tanpa background kotak internal.
- Posisi floating card dioptimalkan untuk desktop, tablet, dan mobile.
