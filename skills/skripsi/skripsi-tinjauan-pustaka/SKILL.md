---
name: skripsi-tinjauan-pustaka
description: Menyusun tinjauan pustaka dan gap penelitian skripsi.
version: 1.0.0
author: Muhammad Alif Abrar, Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [skripsi, tinjauan pustaka, gap, literatur, tabel]
    related_skills: [skripsi-audit-referensi, skripsi-unila-penulisan, skripsi-bahasa-natural]
---

# Tinjauan Pustaka Skripsi

Gunakan skill ini untuk mengubah kumpulan artikel menjadi sintesis yang menunjukkan posisi penelitian. Tabel penelitian terdahulu yang sudah disetujui pembimbing tidak diubah tanpa instruksi baru.

## When to Use

- Menyusun Bab II dan tabel penelitian terdahulu.
- Menentukan persamaan, perbedaan, dan gap penelitian.
- Menghubungkan teori dengan metode penelitian.

## Procedure

1. Kelompokkan sumber berdasarkan objek, metode, data, dan hasil.
2. Catat metadata sumber dari artikel asli.
3. Ringkas tiap sumber pada temuan yang relevan, bukan seluruh isi artikel.
4. Bandingkan data/objek, metode, metrik, skala, dan keterbatasan.
5. Tulis sintesis setelah tabel: apa yang sudah dilakukan dan apa yang belum.
6. Hubungkan gap dengan metode yang benar-benar dipakai penelitian.
7. Pisahkan definisi teori dari uraian algoritma dan hasil penelitian.
8. Audit semua sitasi menggunakan `skripsi-audit-referensi`.

## Struktur tabel

Gunakan kolom yang terbaca dan tidak terlalu padat:

```text
No | Penulis/Tahun | Objek/Data | Metode | Hasil utama | Perbedaan penelitian
```

Jangan menambah kolom jika membuat tabel tidak terbaca. Jika tabel terlalu padat, pecah berdasarkan kelompok literatur dan beri paragraf sintesis.

## Verification

- Setiap baris tabel memiliki sitasi yang valid.
- Ada paragraf sintesis setelah tabel.
- Gap tidak hanya berupa klaim "belum ada penelitian" tanpa batasan pencarian.
- Teori yang dipilih benar-benar dipakai di Bab III.
