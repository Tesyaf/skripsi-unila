---
name: skripsi-audit-format-latex
description: Memeriksa format LaTeX skripsi sesuai panduan UNILA.
version: 1.0.0
author: Muhammad Alif Abrar, Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [skripsi, latex, unila, pdf, format]
    related_skills: [skripsi-unila-penulisan, skripsi-metodologi-komputasional]
---

# Audit Format LaTeX UNILA

Gunakan skill ini untuk mengedit dan memverifikasi proposal atau skripsi LaTeX berdasarkan Panduan Penulisan Karya Ilmiah UNILA. Jangan mengubah isi ilmiah ketika tugasnya hanya format.

## When to Use

- Memperbaiki margin, font, spasi, judul, daftar isi, tabel, gambar, atau kode.
- Mengompilasi PDF dan memeriksa hasilnya.
- Mencari tanda Markdown mentah di LaTeX.

## Aturan inti

- A4; margin kiri 4 cm, atas/kanan/bawah 3 cm.
- Font utama Times 12pt; isi tabel/kode dapat 10–11pt.
- Isi naskah 1,5 spasi; judul/caption/tabel/daftar tertentu 1 spasi.
- Judul bab 6 cm dari tepi atas; kapital, tebal, tengah, tanpa titik.
- Subbab rata kiri, tebal, tanpa titik.
- Alinea indentasi 1 cm dan `\parskip=0pt`.
- Judul tabel di atas tanpa titik; judul gambar di bawah dengan titik.
- Periksa daftar isi, tabel, gambar, dan kode setelah dua kali kompilasi.

## Procedure

1. Baca `preamble.tex` dan file sumber target sebelum mengubah.
2. Cari format yang diatur ganda atau bertentangan.
3. Gunakan `\textit{}` untuk istilah asing; jangan memakai `*...*` Markdown.
4. Gunakan `\texttt{}` untuk nama fungsi, library, dan file.
5. Periksa float agar caption tetap berada pada bagian yang benar.
6. Compile dua kali dengan `pdflatex -interaction=nonstopmode`.
7. Periksa log untuk error, undefined reference, dan overfull box.
8. Ekstrak PDF dengan `pdftotext` atau `pdftohtml` jika posisi perlu diukur.
9. Verifikasi bahwa daftar isi dan daftar gambar/tabel/kode terisi.

## Pitfalls

- Kompilasi sekali setelah menghapus `.aux` membuat daftar kosong.
- `report.cls` dapat menambah jarak ekstra antarbab di LOF/LOT.
- Float dapat berpindah ke subbab berikutnya; gunakan pembatas hanya ketika diperlukan.
- Jangan menyamakan panjang PDF sebagai bukti format benar.
- Jangan menghapus cache LaTeX tanpa memahami dampaknya terhadap daftar dan referensi.

## Verification

- Dua kompilasi selesai tanpa error.
- Tidak ada `LaTeX Error`, `Undefined control sequence`, atau `Emergency stop`.
- Semua daftar terisi.
- Tidak ada tanda Markdown mentah seperti `*italic*` di PDF.
- Posisi judul utama dan jarak penting diperiksa dari PDF, bukan hanya dari source.
