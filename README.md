# 🔐 ARCADIA QUANTUM EA — LICENSE DATABASE

> File ini digunakan sebagai sistem validasi lisensi untuk pengguna **ARCADIA QUANTUM TRADING SYSTEM**.
> EA akan membaca file ini secara otomatis melalui WebRequest untuk memverifikasi akun yang terdaftar.

---

## 📌 FORMAT DATA LISENSI

Setiap baris lisensi menggunakan format berikut:

```
Nama_Pembeli | Nomor_Akun_MT5 | Tanggal_Expired
```

### Contoh:

```
Andre Dharmawangsa | 12345678 | 2026.12.31
Budi Santoso       | 87654321 | 2025.10.01
Siti Rahma         | 99887766 | 2027.01.15
```

---

## ⚠️ ATURAN PENTING

* Gunakan **format tanggal: YYYY.MM.DD**
* Pastikan **tidak ada spasi berlebih**
* Satu akun hanya boleh muncul **1 kali**
* File harus dalam format **plain text (UTF-8)**
* Jangan gunakan karakter aneh atau simbol tambahan

---

## 🔄 UPDATE LISENSI

Untuk menambahkan user baru:

1. Tambahkan baris baru di bawah
2. Gunakan format yang sama
3. Commit perubahan ke repository GitHub
4. EA akan otomatis membaca update dalam ±6 jam

---

## ❌ BLOKIR / CABUT LISENSI

Untuk menonaktifkan lisensi:

* Hapus baris user dari file
  **ATAU**
* Ubah tanggal expired ke tanggal lampau

Contoh:

```
Budi Santoso | 87654321 | 2020.01.01
```

---

## 🔒 KEAMANAN

* Jangan share file ini secara publik jika tidak perlu
* Gunakan repository private jika memungkinkan
* Batasi akses edit hanya untuk admin

---

## 📊 CATATAN

* EA akan tetap berjalan jika:

  * server tidak bisa diakses (menggunakan cache terakhir)
* EA akan berhenti jika:

  * akun tidak ditemukan
  * lisensi expired

---

## 🚀 LISENSI AKTIF

```
Andre Dharmawangsa | 12345678 | 2026.12.31
Budi Santoso       | 87654321 | 2025.10.01
Siti Rahma         | 99887766 | 2027.01.15
```

---

**© 2026 ARCADIA QUANTUM — All Rights Reserved**
