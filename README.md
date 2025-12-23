# Template LaTeX Buku Tugas Akhir Departemen Teknik Informatika ITS

[![latest version](https://img.shields.io/github/v/release/Lab-RPL-ITS/template-buku-ta-if-its)](https://github.com/Lab-RPL-ITS/template-buku-ta-if-its/releases/)
[![commits since latest version](https://img.shields.io/github/commits-since/Lab-RPL-ITS/template-buku-ta-if-its/latest)](https://github.com/Lab-RPL-ITS/template-buku-ta-if-its/commits/master)
[![repo size](https://img.shields.io/github/repo-size/Lab-RPL-ITS/template-buku-ta-if-its)](https://github.com/Lab-RPL-ITS/template-buku-ta-if-its)
[![license](https://img.shields.io/github/license/Lab-RPL-ITS/template-buku-ta-if-its)](./LICENSE)
[![build status](https://img.shields.io/github/actions/workflow/status/Lab-RPL-ITS/template-buku-ta-if-its/ci.yaml?branch=main)](https://github.com/Lab-RPL-ITS/template-buku-ta-if-its/actions/workflows/ci.yaml)

Repositori ini berisi template [LaTeX](https://www.latex-project.org/) lengkap untuk buku tugas akhir yang disesuaikan dengan format resmi [Institut Teknologi Sepuluh Nopember](https://www.its.ac.id/) (ITS). Template ini dirancang untuk memenuhi standar akademik yang ditetapkan berdasarkan [SK Rektor ITS No. 280 Tahun 2022](https://www.its.ac.id/pendidikan/wp-content/uploads/sites/112/2022/03/280-SK-Rektor-ttg-Pedoman-Penyusunan-Laporan-Tugas-Akhir-Sarjana-Sarjana-Terapan.pdf) tentang pedoman penyusunan laporan tugas/proyek akhir program sarjana dan sarjana terapan.

Template ini mencakup semua komponen yang diperlukan untuk buku tugas akhir, mulai dari sampul hingga biografi penulis, dengan format yang telah disesuaikan untuk Departemen Teknik Informatika ITS.

> Contoh file PDF dari template ini bisa dilihat di [sini](https://lab-rpl-its.github.io/template-buku-ta-if-its/buku-ta.pdf).

## Fitur

### Format dan Struktur Dokumen

- Format ukuran halaman A4, margin, dan font Times New Roman sesuai standar ITS
- Struktur dokumen lengkap dengan penomoran halaman yang benar (romawi untuk bagian awal, arab untuk isi)
- Template sampul bahasa Indonesia dan Inggris
- Lembar pengesahan dengan format resmi ITS
- Abstrak dalam bahasa Indonesia dan Inggris
- Pernyataan keaslian dan kode etik akademik

### Komponen Buku Tugas Akhir

- **Pendahuluan**: Latar belakang, rumusan masalah, batasan masalah, tujuan, dan manfaat
- **Tinjauan Pustaka**: Hasil penelitian terdahulu dan dasar teori dengan sistem referensi
- **Desain dan Implementasi**: Rancangan sistem dan implementasi solusi
- **Pengujian dan Analisis**: Hasil pengujian dan analisis yang dilakukan
- **Penutup**: Kesimpulan dan saran untuk pengembangan selanjutnya

### Fitur LaTeX Lanjutan

- Sistem referensi otomatis menggunakan BibLaTeX dengan style APA
- Penomoran gambar, tabel, dan persamaan secara otomatis
- Dukungan untuk code listings dengan syntax highlighting
- Pembuatan daftar isi, daftar gambar, daftar tabel, dan daftar kode sumber otomatis
- Dukungan format gambar JPEG, PNG, dan format lain
- Formatting persamaan matematika yang rapi
- Pengaturan hyphenation bahasa Indonesia

### Automasi dan Tools

- Kompilasi dokumen secara otomatis menggunakan [GitHub Actions](https://github.com/features/actions)
- Sistem cross-reference untuk gambar, tabel, dan persamaan
- Template halaman kosong yang konsisten

## Cara Menggunakan Template

### 1. File Utama

File utama dokumen adalah [`main.tex`](./main.tex) yang mengatur:

- Package LaTeX yang digunakan
- Konfigurasi format dokumen (margin, font, spacing)
- Struktur dokumen dan urutan bab
- Styling untuk judul, referensi, dan numbering

### 2. Struktur Direktori dan File

#### 📁 [`bab/`](./bab) - Isi Buku Tugas Akhir

Berisi file `.tex` untuk setiap bab buku tugas akhir:

- `1-pendahuluan.tex` - Latar belakang, rumusan masalah, tujuan, manfaat
- `2-tinjauan-pustaka.tex` - Penelitian terdahulu dan dasar teori
- `3-metodologi.tex` - Metodologi penelitian
- `4-hasil-dan-pembahasan.tex` - Hasil pengujian dan analisis
- `5-kesimpulan-dan-saran.tex` - Kesimpulan dan saran

#### 📁 [`abstrak/`](./abstrak) - Abstrak

- `abstrak-id.tex` - Abstrak dalam bahasa Indonesia
- `abstrak-en.tex` - Abstrak dalam bahasa Inggris

#### 📁 [`lainnya/`](./lainnya) - Komponen Tambahan

- `lembar-pengesahan.tex` - Halaman pengesahan resmi
- `lembar-pengesahan-en.tex` - Halaman pengesahan bahasa Inggris
- `pernyataan-keaslian.tex` - Pernyataan keaslian karya
- `pernyataan-keaslian-en.tex` - Pernyataan keaslian bahasa Inggris
- `kode-etik.tex` - Pernyataan kode etik akademik
- `kata-pengantar.tex` - Kata pengantar
- `biografi-penulis.tex` - Biografi singkat penulis

#### 📁 [`sampul/`](./sampul) - Halaman Sampul

- `konten-id.tex` - Konten sampul bahasa Indonesia
- `konten-en.tex` - Konten sampul bahasa Inggris
- `sampul-luar.tex` - Template layout sampul luar
- `sampul-luar-tipis.tex` - Template layout sampul dalam
- `gambar/` - Logo dan elemen visual sampul

#### 📁 [`pustaka/`](./pustaka) - Referensi

- `pustaka.bib` - Database referensi dalam format BibTeX
- `variables.tex` - Variabel-variabel yang memuat nama, NRP, judul, dan informasi lainnya
- `tanda-hubung.tex` - Pengaturan hyphenation bahasa Indonesia

#### 📁 [`gambar/`](./gambar) - Aset Visual

Tempat menyimpan gambar, diagram, dan ilustrasi dalam format `.jpg`, `.png`, atau format lain

#### 📁 [`program/`](./program) - Kode Program

Berisi file kode program yang akan dimasukkan pada dokumen dengan syntax highlighting

### 3. Langkah Penggunaan

1. **Personalisasi Data**: Edit informasi mahasiswa, dosen pembimbing, dan judul di file [`pustaka/variables.tex`](./pustaka/variables.tex)
2. **Isi Konten**: Lengkapi setiap file di direktori `bab/` sesuai penelitian Anda
3. **Tambah Referensi**: Masukkan referensi ke `pustaka/pustaka.bib` dalam format BibTeX
4. **Tambah Gambar**: Simpan gambar di direktori `gambar/` dan referensikan di konten
5. **Tambah Kode**: Simpan file kode program di direktori `program/` jika diperlukan
6. **Kompilasi**: Jalankan LaTeX compiler untuk menghasilkan `main.pdf`

### 4. Tips Penggunaan

- Setiap file dilengkapi dengan komentar panduan penggunaan
- Gunakan label dan reference untuk cross-referencing otomatis
- Format sitasi menggunakan `\parencite{}` untuk referensi dalam teks
- Gunakan environment `figure`, `table`, dan `equation` untuk elemen yang perlu dinomori
- Edit variabel di `pustaka/variables.tex` untuk mengubah informasi mahasiswa dan judul

> Penjelasan lengkap dan contoh penggunaan tersedia dalam komentar di setiap file template.

## Persyaratan Sistem

### LaTeX Distribution

Template ini memerlukan distribusi LaTeX yang lengkap seperti:

- **TeX Live** (Linux/Windows/macOS) - Rekomendasi
- **MiKTeX** (Windows)
- **MacTeX** (macOS)

### Package Dependencies

Template menggunakan package LaTeX berikut:

- `geometry` - pengaturan margin dan ukuran halaman
- `setspace` - pengaturan spasi baris
- `biblatex` - manajemen referensi dengan style APA
- `graphicx` - dukungan gambar
- `hyperref` - hyperlink dan bookmark PDF
- `listings` - code syntax highlighting
- `tocloft` - custom table of contents
- `titlesec` - custom section formatting
- `txfonts` - font Times New Roman
- `xcolor` - pewarnaan tabel dan elemen
- `longtable`, `tabularx` - tabel panjang dan fleksibel

### Kompilasi

Untuk menghasilkan dokumen PDF:

```bash
pdflatex main.tex
biber main
```

Atau gunakan `latexmk` untuk kompilasi otomatis:

```bash
latexmk -pdf main.tex
```

## Kontribusi

Kontribusi untuk pengembangan template ini sangat diterima. Silakan:

1. Fork repositori ini
2. Buat branch untuk fitur baru (`git checkout -b feature/nama-fitur`)
3. Commit perubahan (`git commit -am 'Menambah fitur baru'`)
4. Push ke branch (`git push origin feature/nama-fitur`)
5. Buat pull request

## Lisensi

Template ini dilisensikan di bawah [Lisensi MIT](./LICENSE). Anda bebas menggunakan, memodifikasi, dan mendistribusikan template ini untuk keperluan akademik maupun komersial.
