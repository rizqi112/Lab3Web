# Lab3Web - Praktikum 3: CSS Dasar

Laporan Praktikum Pemrograman Web, Universitas Pelita Bangsa.

## Isi Repositori

- lab2_css_dasar.html: dokumen HTML yang berisi CSS internal dan CSS inline
- style_eksternal.css: file CSS eksternal
- screenshots: tangkapan layar setiap langkah praktikum

---

## Langkah 1 - Membuat Dokumen HTML

Pada langkah ini dibuat file lab2_css_dasar.html menggunakan VSCode. Isinya adalah struktur dasar HTML yang terdiri dari header berisi judul h1, navigasi dengan tiga tautan (CSS Dasar, CSS Eksternal, dan HTML Dasar), serta sebuah div dengan id intro yang berisi judul "Hello World", satu paragraf, dan tautan "Informasi selengkapnya" yang memiliki class button dan btn-primary.

Pada tahap ini belum ada CSS sama sekali, sehingga tampilan halaman masih memakai gaya bawaan browser.

![Langkah 1](https://github.com/user-attachments/assets/edbd3c19-3fba-4c1c-8345-b2e45e612239)

## Langkah 2 - Mendeklarasikan CSS Internal

CSS internal ditulis di dalam tag style yang diletakkan pada bagian head. Selector yang dipakai adalah selector elemen, yaitu body, header, h1, dan h1 i (selector turunan untuk teks miring di dalam h1).

Pengaturan yang dilakukan:
- body diberi font Open Sans dengan cadangan sans-serif, serta warna latar abu-abu muda
- header diberi tinggi minimal 80px dan garis bawah berwarna oranye setebal 2px
- h1 diberi ukuran font 26px, warna ungu tua, rata tengah, dan padding 20px 10px
- teks miring pada h1 diberi warna oranye

Aturan h1 berlaku untuk semua elemen h1 pada halaman, sehingga judul "Hello World" juga ikut terkena aturan ini.

![Langkah 2](https://github.com/user-attachments/assets/757483de-c704-4b87-bdc1-d4e232a191fd)

## Langkah 3 - Menambahkan Inline CSS

CSS inline ditulis langsung sebagai atribut style pada tag p, sehingga hanya memengaruhi paragraf tersebut. Paragraf diatur rata tengah dan berwarna putih.

![Langkah 3](https://github.com/user-attachments/assets/94a9732b-6705-4d07-b2c6-d44878975009)

## Langkah 4 - Membuat CSS Eksternal

Dibuat file baru bernama style_eksternal.css yang berisi aturan untuk navigasi, kemudian file tersebut dihubungkan ke dokumen HTML menggunakan tag link pada bagian head.

Pengaturan yang dilakukan:
- nav diberi latar ungu, teks putih, dan padding 12px
- tautan di dalam nav diberi warna putih, tanpa garis bawah, dan padding 10px 20px
- tautan yang aktif atau sedang di-hover diberi warna latar ungu yang lebih gelap

Setelah halaman di-refresh, navigasi tampil sebagai bilah berwarna dengan tautan putih.

![Langkah 4](https://github.com/user-attachments/assets/456a03e8-6ee8-4962-8946-52764cf3c4cd)

## Langkah 5 - Menambahkan CSS Selector (ID dan Class)

Pada file style_eksternal.css ditambahkan dua jenis selector.

ID selector (diawali tanda #):
- #intro diberi latar ungu muda, border 2px, tinggi minimal 100px, dan padding 10px
- #intro h1 dibuat rata kiri, berwarna putih, dan tanpa border. Aturan ini lebih spesifik daripada aturan h1 biasa, sehingga judul "Hello World" tampil berbeda dari judul di header

Class selector (diawali tanda titik):
- .button memberi gaya dasar tombol: padding 15px 20px, warna latar abu-abu, teks putih, tampilan inline-block, margin 10px, tanpa garis bawah, dan sudut membulat
- .btn-primary mengganti warna latar tombol menjadi oranye

Tombol "Informasi selengkapnya" memakai dua class sekaligus, yaitu button dan btn-primary.

![Langkah 5](https://github.com/user-attachments/assets/6fa3c978-ad5a-41b6-b1c6-8640b550dd48)

---

## Eksperimen Perubahan Properti dan Nilai (Tugas No. 1)

Bagian ini mencatat nilai yang saya ubah dari contoh pada modul.

| Bagian | Pada modul | Pada eksperimen |
|---|---|---|
| body | tidak ada warna latar | ditambah warna latar #f7f9fc |
| Border header | 1px solid #77CCEF | 2px solid #F2A65A |
| Font h1 | 24px, warna #0F189F | 26px, warna #7A1F5C |
| Teks miring h1 | #6d6a6b | #F2A65A |
| Warna teks paragraf inline | #ccd8e4 | #ffffff |
| Latar nav | #20A759, padding 10px | #3D2C8D, padding 12px |
| Nav aktif atau hover | #0B6B3A | #2A1D66 |
| Latar #intro | #418fb1, border 1px #099249 | #916BBF, border 2px #3D2C8D |
| .button | tanpa sudut membulat | ditambah sudut membulat 6px |
| .btn-primary | #E42A42 | #F2A65A |
