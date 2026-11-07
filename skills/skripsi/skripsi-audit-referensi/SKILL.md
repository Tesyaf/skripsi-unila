---
name: skripsi-audit-referensi
description: Memeriksa sitasi dan metadata referensi skripsi.
version: 1.0.0
author: Muhammad Alif Abrar, Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [skripsi, referensi, sitasi, metadata, doi]
    related_skills: [skripsi-unila-penulisan, skripsi-revisi-dosen]
---

# Audit Referensi Skripsi

Gunakan skill ini untuk memeriksa kecocokan sitasi dalam naskah dengan daftar pustaka dan metadata sumber. Jangan menyatakan sumber valid hanya karena judulnya terlihat masuk akal.

## When to Use

- Dosen meminta audit referensi.
- Nama penulis, tahun, jurnal, volume, nomor, halaman, atau DOI diragukan.
- Ada sitasi di teks yang tidak muncul di daftar pustaka.
- Jangan menghapus sumber tanpa memeriksa apakah masih disitasi.

## Procedure

1. Ekstrak semua sitasi dari Bab I–V.
2. Ekstrak semua entri daftar pustaka.
3. Cocokkan nama keluarga penulis dan tahun dengan toleransi untuk `dkk.`/`et al.`.
4. Tandai sitasi tanpa entri dan entri tanpa sitasi.
5. Untuk artikel jurnal, verifikasi penulis, tahun, judul, jurnal, volume, nomor, halaman, dan DOI.
6. Untuk website, verifikasi institusi/penulis, judul, tanggal publikasi, URL, dan tanggal akses.
7. Untuk buku, verifikasi penulis, tahun, judul, penerbit, dan kota.
8. Bedakan sumber primer, review, berita, dan dataset resmi.
9. Perbarui LaTeX hanya setelah metadata terverifikasi.
10. Buat laporan status: valid, perlu verifikasi, atau tidak ditemukan.

## Aturan akademik

- Gunakan sumber lama untuk definisi asli atau algoritma asli bila memang sumber primer.
- Tambahkan sumber 5 tahun terakhir untuk perkembangan dan penerapan modern.
- Jangan memakai nama jurnal, portal, atau kota sebagai nama penulis.
- Jangan mengarang volume, nomor, halaman, DOI, atau tanggal.
- Klaim "belum ada penelitian" harus dibatasi pada literatur yang benar-benar ditinjau.

## Verification

- Setiap sitasi memiliki entri daftar pustaka.
- Setiap entri yang dipertahankan digunakan di teks atau ditandai sebagai sumber pendukung.
- Tidak ada metadata yang diisi berdasarkan tebakan.
- DOI/URL dapat dibuka atau diberi status belum terverifikasi.
