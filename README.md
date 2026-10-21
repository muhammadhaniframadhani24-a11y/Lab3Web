# Lab3Web — Praktikum 3 CSS Dasar

**Nama:** Muhammad Hanif Ramadhani  
**NIM:** 312510291  
**Mata Kuliah:** Pemrograman Web

## Tujuan
Praktikum ini bertujuan memahami konsep dasar CSS, aturan penulisan CSS, selector, serta penerapan CSS pada dokumen HTML.

## File Praktikum
- `lab2_css_dasar.html` — halaman HTML dengan CSS internal, inline, dan tautan ke CSS eksternal.
- `style_eksternal.css` — stylesheet eksternal untuk navigasi, ID selector, dan class selector.

## Langkah Praktikum

### 1. Membuat dokumen HTML
Membuat struktur dasar HTML yang berisi header, navigasi, bagian intro, dan footer.

**Screenshot:** Tambahkan screenshot halaman awal di browser di sini.

### 2. Mendeklarasikan CSS Internal
CSS internal diletakkan pada bagian `<head>` di dalam tag `<style>`. Pada halaman ini, CSS internal mengatur font, latar belakang, header, judul, dan tata letak.

**Screenshot:** Tambahkan screenshot tampilan setelah CSS internal diterapkan di sini.

### 3. Menambahkan Inline CSS
Inline CSS ditulis langsung pada atribut `style` sebuah elemen HTML. Contohnya terdapat pada paragraf di bagian intro yang diatur agar rata tengah dan berwarna terang.

**Screenshot:** Tambahkan screenshot setelah inline CSS diterapkan di sini.

### 4. Membuat CSS Eksternal
Aturan CSS eksternal ditulis dalam file `style_eksternal.css`, lalu dihubungkan ke HTML menggunakan tag `<link>` pada bagian `<head>`.

**Screenshot:** Tambahkan screenshot setelah CSS eksternal diterapkan di sini.

### 5. Menambahkan CSS Selector
- **Element selector** memilih elemen berdasarkan nama tag, misalnya `body` atau `nav`.
- **ID selector** menggunakan tanda `#`, misalnya `#intro`, untuk menargetkan elemen dengan ID tersebut.
- **Class selector** menggunakan tanda titik `.`, misalnya `.button` dan `.btn-primary`, untuk menargetkan elemen berdasarkan class.

**Screenshot:** Tambahkan screenshot hasil ID dan class selector di sini.

## Jawaban Pertanyaan Praktikum

### 1. Eksperimen properti dan nilai CSS
Pada halaman ini dilakukan eksperimen dengan properti `font-family`, `background-color`, `color`, `padding`, `border`, `border-radius`, `text-align`, `line-height`, dan `box-shadow`. Properti tersebut digunakan untuk mengatur jenis huruf, warna, jarak, garis tepi, perataan teks, dan bayangan.

### 2. Perbedaan `h1 { ... }` dengan `#intro h1 { ... }`
`h1 { ... }` memilih semua elemen `<h1>` pada halaman. Sementara itu, `#intro h1 { ... }` hanya memilih elemen `<h1>` yang berada di dalam elemen dengan `id="intro"`. Selector yang lebih spesifik tersebut dapat mengatur judul di bagian intro secara berbeda dari judul lainnya.

### 3. CSS internal, eksternal, dan inline pada elemen yang sama
Jika ketiganya mengatur properti yang sama pada elemen yang sama, aturan CSS inline biasanya menang atas aturan internal dan eksternal, selama tidak ada aturan `!important` atau kondisi khusus lain yang mengubah prioritas. Contoh: aturan eksternal `p { color: blue; }`, aturan internal `p { color: green; }`, dan elemen `<p style="color: red;">Teks</p>`. Teks akan berwarna merah karena aturan inline diterapkan langsung pada elemen. Jika aturan internal dan eksternal memiliki tingkat kepentingan dan spesifisitas yang sama, urutan deklarasi juga dapat menentukan hasil.

### 4. Elemen memiliki ID dan class
Jika elemen `<p id="paragraf-1" class="text-paragraf">` terkena aturan `#paragraf-1 { color: red; }` dan `.text-paragraf { color: blue; }`, warna teks menjadi merah karena selector ID memiliki spesifisitas lebih tinggi daripada selector class. Namun, untuk properti yang berbeda, kedua aturan dapat diterapkan sekaligus.

## Validasi CSS
Validasi CSS dapat dilakukan melalui [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/). Unggah file `style_eksternal.css` atau masukkan URL setelah halaman dipublikasikan, lalu periksa pesan validasi.

## Cara Menjalankan
1. Buka folder ini di Visual Studio Code.
2. Buka `lab2_css_dasar.html` di browser, atau jalankan dengan ekstensi Live Server.
3. Pastikan `style_eksternal.css` berada di folder yang sama dengan file HTML.
4. Ambil screenshot hasil setiap tahap praktikum dan masukkan ke README ini.
5. Commit dan push seluruh file ke repository GitHub bernama `Lab3Web`.

## Catatan Screenshot
Screenshot harus diambil dari hasil praktik yang benar-benar dijalankan. Ganti petunjuk screenshot di atas dengan gambar milik sendiri sebelum mengumpulkan laporan.

