---
name: skripsi-unila-penulisan
description: Menulis skripsi UNILA dengan struktur dan gaya akademik.
version: 1.0.0
author: Muhammad Alif Abrar, Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [skripsi, unila, penulisan, akademik, latex]
    related_skills: [skripsi-revisi-dosen, skripsi-bahasa-natural, skripsi-audit-referensi]
---

# Penulisan Skripsi UNILA

Gunakan skill ini untuk menyusun atau menata proposal dan skripsi Universitas Lampung. Skill ini mengatur struktur argumentasi, hubungan antarbagian, dan gaya bahasa; aturan jurusan atau pembimbing tetap menjadi prioritas.

## When to Use

- Menulis Bab I, Bab II, Bab III, simpulan, atau abstrak.
- Menata hubungan masalah, tujuan, metode, dan kontribusi.
- Memeriksa apakah isi sesuai dengan Panduan UNILA.
- Jangan gunakan untuk memverifikasi metadata sumber; gunakan `skripsi-audit-referensi`.

## Struktur inti

- **Bab I:** masalah, data/fenomena, formulasi masalah, solusi, rumusan masalah, batasan, tujuan, manfaat.
- **Bab II:** penelitian terdahulu, teori yang dipakai, algoritma, rumus, dan gap penelitian.
- **Bab III:** data, alat, tahapan, implementasi, pengujian, metrik, dan evaluasi.
- **Bab IV:** hasil berdasarkan skenario dan metrik yang telah didefinisikan.
- **Bab V:** jawaban rumusan masalah, keterbatasan, dan saran yang dapat dikerjakan.

## Procedure

1. Baca aturan universitas, panduan fakultas, dan catatan pembimbing.
2. Tulis masalah penelitian dalam satu kalimat yang dapat diuji.
3. Jelaskan mengapa masalah itu penting sebelum menyebut algoritma.
4. Hubungkan data, objek, model matematis, metode, dan metrik secara berurutan.
5. Pastikan setiap tujuan memiliki hasil atau metrik yang dapat diperiksa.
6. Bedakan teori, metode penelitian, hasil, dan interpretasi.
7. Periksa bahwa setiap istilah teknis didefinisikan saat pertama kali dipakai.
8. Verifikasi bahwa semua sitasi memiliki entri daftar pustaka.

## Gaya bahasa

- Tulis kalimat aktif, spesifik, dan tidak bertele-tele.
- Hindari pembuka generik seperti "di era digital" atau "sangat penting" tanpa bukti.
- Jangan membuat klaim baru ketika memparafrase.
- Istilah asing dicetak miring; nama fungsi, library, dan kode memakai `\texttt{}`.
- Gunakan satu istilah secara konsisten: `kinerja`, bukan bergantian dengan `performa`.
- Jangan menyatakan metode sebagai optimal jika penelitian hanya menguji heuristik.

## Verification

- Rumusan masalah, tujuan, batasan, metode, dan metrik saling cocok.
- Tidak ada detail implementasi Python di Batasan Masalah.
- Latar belakang sekitar 3–4 halaman atau sesuai arahan pembimbing.
- Setiap tabel/gambar dirujuk dalam teks dan memiliki caption.
