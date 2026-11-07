# Skills Skripsi UNILA

Kumpulan skill untuk membantu penulisan dan pengerjaan skripsi Universitas Lampung. Skill ini dibuat untuk dipakai di Hermes Agent dan dapat digunakan secara terpisah atau bersama-sama.

Repository: <https://github.com/Tesyaf/skripsi-unila>

## Isi repository

- `skripsi-unila-penulisan` — struktur, gaya, dan alur penulisan skripsi.
- `skripsi-revisi-dosen` — mengubah catatan pembimbing menjadi daftar tindakan.
- `skripsi-bahasa-natural` — parafrasa dari gagasan penulis tanpa gaya AI generik.
- `skripsi-audit-referensi` — mencocokkan sitasi dan metadata daftar pustaka.
- `skripsi-metodologi-komputasional` — menyusun Bab III algoritma dan eksperimen.
- `skripsi-audit-format-latex` — memeriksa LaTeX dan PDF sesuai aturan UNILA.
- `skripsi-tinjauan-pustaka` — menyusun sintesis, persamaan, perbedaan, dan gap.

Skill ini berisi workflow umum. Sesuaikan nama fakultas, program studi, dataset, algoritma, dan aturan pembimbing.

## Persyaratan

- Hermes Agent sudah terpasang.
- Koneksi internet saat instalasi.
- Tidak perlu memasukkan password atau token ke prompt skill.

## Instalasi cepat: semua skill

Tambahkan repository ini sebagai sumber skill:

```bash
hermes skills tap add Tesyaf/skripsi-unila
```

Lalu instal skill yang diperlukan:

```bash
hermes skills install Tesyaf/skripsi-unila/skripsi-unila-penulisan
hermes skills install Tesyaf/skripsi-unila/skripsi-revisi-dosen
hermes skills install Tesyaf/skripsi-unila/skripsi-bahasa-natural
hermes skills install Tesyaf/skripsi-unila/skripsi-audit-referensi
hermes skills install Tesyaf/skripsi-unila/skripsi-metodologi-komputasional
hermes skills install Tesyaf/skripsi-unila/skripsi-audit-format-latex
hermes skills install Tesyaf/skripsi-unila/skripsi-tinjauan-pustaka
```

Cek hasil instalasi:

```bash
hermes skills list
hermes skills search skripsi
```

## Instalasi satu skill dari URL

Jika hanya membutuhkan satu skill:

```bash
hermes skills install https://raw.githubusercontent.com/Tesyaf/skripsi-unila/main/skills/skripsi/skripsi-unila-penulisan/SKILL.md
```

Ganti bagian akhir URL dengan nama skill yang diperlukan.

## Memuat skill saat chat

Muat satu skill untuk satu sesi:

```bash
hermes --skills skripsi-unila-penulisan
```

Muat beberapa skill sekaligus:

```bash
hermes --skills skripsi-unila-penulisan,skripsi-bahasa-natural,skripsi-audit-referensi
```

Untuk satu pertanyaan:

```bash
hermes chat -q "Periksa apakah latar belakang saya fokus pada problem solving." \
  --skills skripsi-unila-penulisan,skripsi-revisi-dosen
```

## Bundle opsional untuk workflow skripsi

Setelah semua skill terpasang, buat bundle sekali:

```bash
hermes bundles create skripsi-unila \
  --description "Workflow penulisan dan revisi skripsi UNILA" \
  --instruction "Gunakan aturan pembimbing dan fakta penelitian pengguna sebagai sumber utama." \
  --skill skripsi-unila-penulisan \
  --skill skripsi-revisi-dosen \
  --skill skripsi-bahasa-natural \
  --skill skripsi-audit-referensi \
  --skill skripsi-metodologi-komputasional \
  --skill skripsi-audit-format-latex \
  --skill skripsi-tinjauan-pustaka
```

Cek bundle:

```bash
hermes bundles list
hermes bundles show skripsi-unila
```

Gunakan bundle dalam chat dengan slash command:

```text
/skripsi-unila
```

## Contoh penggunaan

### Menyusun Bab I

```text
Gunakan skill skripsi-unila-penulisan. Bantu susun Latar Belakang dari draf saya. Pertahankan fakta dan jangan menambah referensi yang belum diverifikasi.
```

### Menindaklanjuti catatan dosen

```text
Gunakan skripsi-revisi-dosen. Ubah catatan bimbingan ini menjadi checklist file, bagian, tindakan, dan status verifikasi.
```

### Parafrasa natural

```text
Gunakan skripsi-bahasa-natural. Rapikan paragraf ini dari gagasan saya sendiri. Jangan menambah klaim atau sitasi baru.
```

### Audit referensi

```text
Gunakan skripsi-audit-referensi. Cocokkan seluruh sitasi Bab I–III dengan Daftar Pustaka dan tandai metadata yang belum terverifikasi.
```

### Audit PDF LaTeX

```text
Gunakan skripsi-audit-format-latex. Compile dua kali, periksa daftar isi dan daftar gambar, lalu cari error dan tanda Markdown mentah di PDF.
```

## Pembaruan skill

Perbarui daftar sumber dan instalasi sesuai versi Hermes yang dipakai:

```bash
hermes skills tap list
hermes skills update
hermes skills check
```

Jika instalasi dari tap tidak menemukan skill, gunakan URL `raw.githubusercontent.com` langsung atau periksa bahwa repository publik memiliki branch `main`.

## Privasi

Repository ini hanya berisi skill, README, lisensi, dan `.gitignore`. Jangan mengunggah:

- naskah skripsi pribadi;
- PDF sempro;
- dataset;
- token, password, atau file `.env`;
- hasil eksperimen yang memuat data pribadi;
- path lokal pengguna.

## Lisensi

Skill dan dokumentasi repository ini dirilis dengan lisensi MIT. Lihat `LICENSE`.
