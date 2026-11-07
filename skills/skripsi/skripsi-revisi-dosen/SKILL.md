---
name: skripsi-revisi-dosen
description: Mengubah catatan dosen menjadi revisi skripsi yang terukur.
version: 1.0.0
author: Muhammad Alif Abrar, Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [skripsi, revisi, dosen, pembimbing, akademik]
    related_skills: [skripsi-unila-penulisan, skripsi-bahasa-natural]
---

# Revisi Dosen Skripsi

Gunakan skill ini ketika menerima catatan lisan, tulisan tangan, atau komentar PDF dari dosen pembimbing. Hasilnya harus berupa daftar tindakan yang dapat diverifikasi, bukan sekadar parafrasa komentar.

## When to Use

- Catatan dosen meminta fokus masalah, pemadatan latar belakang, atau penguatan metodologi.
- Komentar meminta flowchart, tabel algoritma, contoh perhitungan, atau perbaikan referensi.
- Jangan menganggap tulisan tangan yang buram sebagai fakta; tandai bagian yang tidak terbaca.

## Procedure

1. Transkripsikan catatan yang benar-benar terbaca dan tandai kata yang tidak pasti.
2. Kelompokkan catatan menjadi isi, struktur, bahasa, referensi, dan format.
3. Petakan setiap catatan ke file dan bagian yang terdampak.
4. Buat checklist dengan tiga status: belum dikerjakan, sudah dikerjakan, perlu verifikasi.
5. Revisi isi berdasarkan gagasan penulis; jangan menambah klaim yang tidak didukung sumber.
6. Periksa konsistensi istilah, angka, tanggal, nama algoritma, dan dataset.
7. Compile atau render dokumen dan periksa hasil visual.
8. Laporkan bagian yang masih membutuhkan keputusan pembimbing.

## Pola revisi yang umum

- **"Latar belakang terlalu panjang"**: pertahankan masalah, bukti, gap, solusi, dan kontribusi; pindahkan detail teknis ke Bab II/III.
- **"Fokus problem"**: jelaskan alur fenomena → kendala → model → metode → evaluasi.
- **"Beri contoh"**: tambahkan contoh numerik yang diberi label ilustrasi jika bukan data nyata.
- **"Beri flowchart"**: tampilkan input, proses, keputusan, loop, output, dan validasi.
- **"Lengkapi tabel"**: cek penulis, tahun, objek/data, metode, hasil, persamaan, perbedaan, dan gap.
- **"Cek ulang"**: cocokkan teks, kode, tabel, gambar, dan daftar pustaka; jangan hanya memperbaiki ejaan.

## Verification

- Setiap komentar dosen memiliki tindakan dan lokasi file.
- Revisi tidak mengubah makna data atau metode tanpa persetujuan.
- Semua angka di naskah dapat dilacak ke dataset atau output eksperimen.
- PDF final dikompilasi ulang dan checklist ditutup dengan bukti.
