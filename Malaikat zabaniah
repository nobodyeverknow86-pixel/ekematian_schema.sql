# eKematian

Sistem pengurusan ahli, kematian, dan bayaran untuk pertubuhan menggunakan Android/SQLite.  
Struktur database lengkap, mudah digunakan, dan siap untuk penambahbaikan masa depan.

---

## Ciri-ciri Utama

- **Pengurusan Ahli & Pertubuhan**
  - Tambah, kemaskini, dan paparan maklumat ahli.
  - Paparan profil pertubuhan (logo, visi, misi, latar belakang).
- **Bayaran & Transaksi**
  - Rekod bayaran ahli, resit, dan status pembayaran.
- **Kematian**
  - Rekod kematian, sebab, dan senarai ahli meninggal.
- **Waris**
  - Simpan maklumat waris bagi setiap peserta.
- **Playlist & Lagu**
  - Boleh upload lagu latar, paparan playlist.
- **Emergency**
  - Butang emergency untuk setiap peserta dan peserta belum bayar.
  - Log tindakan emergency.
- **Paparan Mesra Pengguna**
  - Boleh "hide" maklumat sensitif (IC, alamat, no waris) dari paparan umum.
  - Warna/gambar latar boleh diubah admin.
- **Sekuriti**
  - Password hash, kawalan akses maklumat sensitif.

---

## Struktur Database

Semua jadual utama telah disepadukan:
- `admin`
- `pertubuhan`
- `playlist`
- `peserta`
- `waris`
- `transaksi`
- `kematian`
- `emergency_log`

Skrip penuh SQL: [`ekematian_schema.sql`](ekematian_schema.sql)

---

## Cara Guna (Android/SQLite)

1. **Salin skrip** `ekematian_schema.sql` ke projek anda.
2. **Import** ke SQLite (contoh guna DB Browser for SQLite, atau dalam Room Migration).
3. **Integrasi ke aplikasi Android**:
    - Boleh guna Room, SQLiteOpenHelper, atau library ORM Android lain.
    - Untuk auto-generate no keahlian gunakan logik di aplikasi (`EKM-YYMMDD-ID`).
    - Untuk sekuriti, pastikan hash password dan kawal akses field sensitif di app/backend.

---

## Contoh Skrip Import (Android Room/SQLiteOpenHelper)
```java
// Contoh Room migration
db.execSQL(FileUtils.readFileFromAssets("ekematian_schema.sql"));
```

---

## Nota & Penyesuaian

- **Jangan papar maklumat sensitif** (IC, alamat, no tel, waris) di paparan umum.
- Emergency, pembayaran, dan hide info telah tersedia di struktur DB.
- Untuk kemudahan testing/demo, boleh tambah data contoh (dummy) jika perlu.

---

## Sumbangan
Pull request dan penambahbaikan dialu-alukan!

---

## Lesen
Sila rujuk fail LICENSE.
