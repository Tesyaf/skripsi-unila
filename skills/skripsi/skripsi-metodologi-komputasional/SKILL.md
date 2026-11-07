---
name: skripsi-metodologi-komputasional
description: Menyusun metodologi skripsi algoritma dan eksperimen.
version: 1.0.0
author: Muhammad Alif Abrar, Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [skripsi, metodologi, algoritma, eksperimen, dataset]
    related_skills: [skripsi-unila-penulisan, skripsi-revisi-dosen]
---

# Metodologi Komputasional

Gunakan skill ini untuk menyusun Bab III penelitian yang mengembangkan, menerapkan, atau membandingkan algoritma. Isi harus dapat direproduksi dari dataset, kode, parameter, dan metrik yang disebutkan.

## When to Use

- Menulis bagian jenis data, alat, tahapan, implementasi, pengujian, atau evaluasi.
- Menjelaskan algoritma dari pseudocode dan kode yang benar-benar dijalankan.
- Menyusun flowchart atau tabel tahapan.

## Struktur yang disarankan

1. Jenis dan sumber data.
2. Waktu dan tempat penelitian.
3. Alat dan bahan.
4. Tahapan penelitian.
5. Pra-pemrosesan.
6. Perhitungan jarak atau fitur.
7. Konstruksi algoritma.
8. Validasi hasil.
9. Optimasi atau pencarian lokal.
10. Pengujian dan evaluasi.

## Procedure

1. Catat sumber, tanggal pengamatan, tanggal unduh, wilayah, format, atribut, dan ukuran dataset.
2. Tulis urutan pra-pemrosesan sama dengan urutan kode.
3. Jelaskan input, output, kondisi, loop, dan kriteria terminasi setiap algoritma.
4. Pisahkan algoritma utama, metode pembanding, dan metode perbaikan.
5. Definisikan metrik sebelum membahas hasil.
6. Jelaskan validasi struktur dan validasi nilai.
7. Catat parameter eksperimen dan jangan menulis parameter yang tidak dijalankan.
8. Buat flowchart yang mengikuti pseudocode, bukan alur ideal yang berbeda dari kode.
9. Hubungkan setiap gambar, tabel, dan kode dengan uraian sebelum atau sesudahnya.

## Untuk penelitian rute

- Definisikan objek sebagai simpul dan jarak sebagai bobot sisi.
- Jelaskan apakah graf lengkap, berarah/tak berarah, dan berbobot.
- Jelaskan apakah rute kembali ke titik awal.
- Jelaskan asumsi yang tidak dimodelkan: jalan, topografi, kapasitas, waktu pelayanan, atau multi-armada.
- Validasi tur dengan derajat simpul dan keterhubungan.
- Laporkan total panjang rute, waktu eksekusi, iterasi perbaikan, dan skenario data.

## Verification

- Pembaca dapat mengulang eksperimen dari Bab III dan kode.
- Semua angka berasal dari dataset atau output eksekusi.
- Pseudocode, flowchart, dan implementasi tidak saling bertentangan.
- Tidak ada klaim optimal jika metode hanya heuristik.
