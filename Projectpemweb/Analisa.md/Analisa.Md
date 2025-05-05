# 🔍 METODE ANALISIS SISTEM DIGITAL PERUSAHAAN PENDIDIKAN (SPESIFIK UNTUK DEVELOPER)

## 📌 TUJUAN
Membangun sistem digital berbasis web yang terdiri dari:
- Company Profile
- Human Resource Management (HRM)
- Learning Management System (LMS)
- API Services

---

## ✅ 1. ANALISIS KEBUTUHAN (Requirement Analysis)

### 📌 Teknik:
- Wawancara Admin Company, HCM, dan LMS
- Studi dokumen operasional manual
- Benchmark sistem LMS/HRM modern

### 📌 Hasil:
**User Role & Modul yang dibutuhkan:**

| Role         | Modul yang Diakses                                     |
|--------------|--------------------------------------------------------|
| Admin Company| Home, About Us, Blog, Contact Us, Testimoni            |
| Admin HRM    | Pegawai, Departemen, Cabang, Absensi, Gaji, Cuti, Event|
| Admin LMS    | Siswa, Guru, Modul, Quiz, Nilai, Sertifikat, Pembayaran, Notifikasi|
| Siswa        | Modul, Quiz, Nilai, Sertifikat                         |
| Guru         | Modul, Nilai, Quiz                                     |

---

## ✅ 2. ANALISIS PIECES (Fokus Teknologi)

| Aspek       | Permasalahan Saat Ini                 | Solusi Digital yang Diberikan         |
|-------------|----------------------------------------|----------------------------------------|
| Performance | Absensi manual, penggajian lama        | Otomatisasi absensi dan slip gaji     |
| Information | Modul/manual disimpan terpisah         | Centralized module system             |
| Economy     | Biaya operasional tinggi (manual)      | Hemat biaya cetak & kertas            |
| Control     | Tidak ada hak akses                    | Multi-role system + autentikasi token |
| Efficiency  | Banyak pengulangan tugas (pengiriman materi, slip gaji) | Otomatisasi proses |
| Service     | Kurang notifikasi ke user              | Email & WhatsApp notification system  |

---

## ✅ 3. ANALISIS SWOT (TEKNIS)

| Kategori      | Detail Spesifik untuk Developer |
|---------------|-------------------------------|
| **Strength**  | Laravel ecosystem kuat, bisa gunakan package Laravel Cashier, Sanctum, DomPDF, Midtrans |
| **Weakness**  | Ketergantungan pada layanan pihak ketiga (Midtrans, WA API), butuh dokumentasi rapi |
| **Opportunity** | API bisa dijual sebagai SaaS ke lembaga lain (multitenancy) |
| **Threat**    | Jika token API tidak aman, bisa bocor data siswa/gaji |

---

## ✅ 4. ANALISIS 5W1H (DEVELOPER-FRIENDLY)

| Aspek | Detail Teknis |
|-------|---------------|
| **What** | Sistem Web Laravel + MySQL + Midtrans + WhatsApp API |
| **Why**  | Untuk digitalisasi total operasional lembaga pendidikan |
| **Who**  | 4 Role utama (Admin Company, Admin HRM, Admin LMS, Siswa/Guru) |
| **Where** | Diakses melalui domain utama (subdomain untuk admin bisa dibuat) |
| **When**  | Dikerjakan dalam 3 fase: desain → development → testing |
| **How**   | Modular Laravel Project, MVC Pattern, REST API, Token Auth |

---

## ✅ 5. USE CASE UTAMA (UNTUK UML & KODING)

### 📌 Modul: HRM (Admin HCM)

- **Manage Pegawai**
  - `GET /pegawai`
  - `POST /pegawai`
  - `PUT /pegawai/{id}`
  - `DELETE /pegawai/{id}`

- **Absensi**
  - Pegawai absen → `POST /absensi`
  - Admin lihat rekap → `GET /absensi?date=`

- **Gaji**
  - Generate slip otomatis → `POST /gaji/generate`
  - Download slip → `GET /gaji/download/{id}`

---

### 📌 Modul: LMS (Admin LMS)

- **Modul Pembelajaran**
  - `GET /modul`
  - `POST /modul`
  - `PUT /modul/{id}`
  - File: Upload PDF/Video (disimpan di storage Laravel)

- **Quiz & Nilai**
  - Guru buat quiz → `POST /quiz`
  - Siswa jawab → `POST /quiz/jawab`
  - Penilaian otomatis/manual

- **Sertifikat**
  - Setelah siswa lulus: `GET /sertifikat/{id}` → hasilkan PDF

- **Pembayaran**
  - Integrasi Midtrans: token dari Snap, webhook listener

- **Notifikasi**
  - Email: SMTP (Mailtrap/Gmail Sendgrid)
  - WhatsApp: Kirim API `POST /notif/wa`

---

## ✅ 6. ARSITEKTUR SISTEM

