# AGENTS.md — Kelompok 7 (TK1 Lab Sains Data)

Panduan ringkas khusus agen AI yang bekerja pada repositori proyek Kelompok 7.

## 1. Konteks Proyek & Keputusan
- **Topik**: Penentuan Prioritas Wilayah Mitigasi Banjir dan Tanah Longsor di Jawa Tengah Berbasis Data Kejadian dan Dampak per Penduduk (2020–2025).
- **Pertanyaan Utama**: Kabupaten/kota mana di Jawa Tengah yang sebaiknya didahulukan untuk program mitigasi banjir dan tanah longsor?
- **Keputusan yang Dihasilkan**: Menetapkan 5 kabupaten/kota prioritas sebelum penyusunan anggaran tahun berikutnya dengan membandingkan:
  1. **Alternatif A**: Jumlah kejadian banjir dan tanah longsor terbanyak.
  2. **Alternatif B**: Dampak bencana per 100.000 penduduk (korban terdampak dan rumah rusak).
  3. **Alternatif C**: Mempertahankan pola alokasi penanganan merata saat ini.
- **Tim Kelompok 7**: Shabrina Aisyah Aulia, Nisazka Syaula Hapsari, dan Fitra Dya Bela Ivanto (detail di `00-admin/anggota.md`).

## 2. Batasan Ketat
- **Rahasia & Kredensial**: Dilarang menulis kunci API, token, atau sandi di berkas mana pun. Simpan seluruh kredensial hanya di `.env` (sudah diabaikan oleh `.gitignore`).
- **Privasi & PII**: Dilarang memasukkan informasi identitas pribadi (PII) orang sungguhan, termasuk nama korban, nomor HP, email, alamat, maupun NIK.
- **Klasifikasi Data**: Hanya olah data **Hijau/agregat** (misalnya agregat per kabupaten/kota dari sumber resmi/publik).
- **Integritas Data Mentah**: Dilarang mengubah atau menimpa isi folder `data/mentah/`. Gunakan `data/mentah/` hanya sebagai sumber baca lokal (tidak untuk di-commit).
- **Akurasi Fakta**: Dilarang mengarang angka, hasil perhitungan, atau tautan sumber.
- **Bukti Kutipan**: Setiap kutipan dari ulasan, portal data, atau dasbor wajib disertai tangkapan layar bertanggal yang disimpan di `00-admin/bukti/`.
- **Penghapusan Berkas**: Dilarang menghapus berkas apa pun tanpa izin eksplisit dari anggota tim.

## 3. Struktur Folder Repo
- `README.md` — Ringkasan proyek, tujuan, dan alternatif keputusan.
- `00-admin/` — Administrasi kelompok (`anggota.md`) dan bukti tangkapan layar bertanggal di `00-admin/bukti/`.
- `01-riset/` — Catatan riset, eksplorasi awal, dan dokumentasi sumber data.
- `data/sampel/` — Sampel data agregat/non-sensitif yang aman disimpan di Git (`data/mentah/` bersifat lokal dan diabaikan Git).
- `.opencode/skills/` — Skill khusus proyek untuk agen AI.

## 4. Kebiasaan Pencatatan (`LOG-AI.md`)
Setiap selesai pekerjaan penting bersama AI, catat entri baru di `LOG-AI.md` dengan format kolom berikut:
- **Tanggal**: Waktu pengerjaan (YYYY-MM-DD).
- **Anggota**: Nama anggota kelompok yang mengarahkan.
- **Perintah**: Ringkasan instruksi yang diberikan ke AI.
- **Hasil**: Ringkasan output/perubahan yang dihasilkan.
- **Yang dicek/diperbaiki manusia**: Bagian yang diverifikasi, dikoreksi, atau disesuaikan oleh anggota kelompok.
