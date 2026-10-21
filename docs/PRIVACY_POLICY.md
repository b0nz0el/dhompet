# Kebijakan Privasi (Privacy Policy) - dhompet

Terakhir diperbarui: 21 Oktober 2026

Aplikasi **dhompet** ("kami", "aplikasi", atau "dhompet") berkomitmen penuh untuk melindungi privasi Anda. Kebijakan Privasi ini menjelaskan bagaimana informasi Anda dikelola saat menggunakan aplikasi **dhompet** (dengan Application ID: `id.dhompet.app`).

---

## 1. Prinsip Utama: Arsitektur "Local-First" (Privasi Total)
Aplikasi **dhompet** dibangun dengan prinsip **Local-First / Offline-First**. Seluruh data keuangan pribadi Anda—termasuk daftar akun, saldo, rincian transaksi, kategori, anggaran belanja, dan catatan hutang-piutang—disimpan **secara lokal di perangkat Anda sendiri** dan **TIDAK PERNAH dikirimkan ke server kami atau pihak ketiga manapun**.

Kami **tidak memiliki server database sentral**, kami **tidak menjual**, dan kami **tidak memonetisasi data pribadi Anda**.

---

## 2. Informasi yang Disimpan di Perangkat Anda
Data berikut disimpan secara aman dalam database lokal (SQLite Room Database) di ruang penyimpanan privat (*sandbox*) perangkat Anda:
- Nama panggilan atau nama profil yang Anda masukkan saat pertama kali membuka aplikasi.
- Riwayat transaksi (pemasukan, pengeluaran, transfer).
- Daftar rekening, dompet fisik, atau kartu yang Anda buat.
- Kategori dan anggaran bulanan.

Data ini sepenuhnya berada di bawah kendali Anda. Jika Anda menghapus aplikasi dari perangkat Anda tanpa melakukan ekspor cadangan (*backup*), data tersebut akan terhapus oleh sistem operasi Android.

---

## 3. Fitur Pencadangan (Backup & Restore)
- Fitur pencadangan memungkinkan Anda mengekspor data ke dalam berkas terenkripsi/zip di memori internal perangkat Anda.
- Anda memiliki kebebasan penuh untuk menyimpan berkas cadangan ini di media penyimpanan pribadi Anda (misalnya Google Drive pribadi, email, atau kartu SD).
- Kami tidak memiliki akses terhadap berkas cadangan yang Anda buat.

---

## 4. Penggunaan Jaringan Internet
Aplikasi hanya menggunakan koneksi internet untuk dua tujuan teknis non-pribadi:
1. **Pembaruan Nilai Tukar Kurs (Exchange Rates)**: Jika Anda menggunakan mata uang asing, aplikasi akan meminta data nilai tukar mata uang publik dari API terbuka (`currency-api.pages.dev`). Permintaan ini tidak menyertakan informasi identitas atau saldo Anda.
2. **Laporan Crash & Kinerja (Opsional)**: Aplikasi dapat menggunakan layanan analitik kesalahan standar (Firebase Crashlytics) untuk mendeteksi kerusakan teknis agar bug dapat segera diperbaiki. Laporan crash tidak memuat data transaksi keuangan Anda.

---

## 5. Izin Perangkat (Permissions)
Aplikasi hanya meminta izin yang mutlak diperlukan untuk fungsionalitas aplikasi:
- `POST_NOTIFICATIONS`: Digunakan untuk mengirimkan pengingat pencatatan transaksi harian yang dapat Anda aktifkan/nonaktifkan kapan saja di menu Pengaturan.
- `RECEIVE_BOOT_COMPLETED` & `SET_ALARM`: Digunakan untuk menjadwalkan pembayaran terencana dan notifikasi pengingat tepat waktu saat ponsel dinyalakan ulang.

---

## 6. Hak Pengguna & Penghapusan Data
Karena seluruh data tersimpan di ponsel Anda:
- Anda dapat menyunting atau menghapus data transaksi kapan saja.
- Anda dapat menghapus seluruh data seketika melalui menu **Pengaturan ➔ Zona Bahaya ➔ Hapus Semua Data Pengguna**, atau cukup dengan melakukan *Clear Data* / *Uninstall* aplikasi.

---

## 7. Kontak Kami
Jika Anda memiliki pertanyaan terkait Kebijakan Privasi ini, silakan hubungi kami melalui repositori proyek atau email pengembang.

---
*Dhompet - Manajer Keuangan Pribadi yang Aman, Nyaman, dan Terpercaya.*
