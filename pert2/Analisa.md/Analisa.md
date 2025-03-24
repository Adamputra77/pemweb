
## **Analisis Lengkap dari Semua Perintah Menggunakan 5W1H & SWOT**

### **1. 5W1H ANALYSIS**

#### **1. What (Apa?)**

**Perintah yang diberikan:**

- Mempelajari HTML dasar.
- Menjalankan layanan dalam **OS di dalam OS** menggunakan **Docker** dan **VPS Ubuntu 22**.
- Menggunakan **XAMPP, VS Code, Postman, Navicat, WSL** dalam VPS.
- Membuat sistem folder dan file konfigurasi dalam proyek (`pert1/nginx/nginx.conf`, `pert1/src/.env`, `docker-compose.yml`, `index.html`).
- Menggunakan **Nginx Proxy Manager** untuk mengelola server.
- Membangun **website portfolio** sebagai proyek UTS/UAS.
- Menyiapkan **company profile** untuk proyek akhir dengan **100 kasus yang berbeda**.

#### **2. Why (Mengapa?)**

- **HTML** adalah dasar dari semua website dan harus dipahami sebelum lanjut ke teknologi lain.
- **Docker** mempermudah deployment dengan **isolasi lingkungan** (APP, DB, Nginx).
- **Nginx Proxy Manager** digunakan untuk menangani **routing traffic** dan meningkatkan performa.
- **VPS Ubuntu 22** dipilih sebagai server untuk meniru lingkungan produksi nyata.
- **Proyek UTS/UAS** bertujuan untuk membangun **portfolio profesional** dan pengalaman praktik.
- **Company profile** sebagai proyek akhir membantu dalam membangun **sistem skala besar** dengan berbagai kasus berbeda.

#### **3. When (Kapan?)**

- **Belajar HTML** dimulai dari pertemuan kedua.
- **Pembuatan struktur proyek** dilakukan sejak awal (pembuatan folder, konfigurasi Docker & Nginx).
- **Portfolio untuk UTS/UAS** dibuat setelah memahami HTML dasar.
- **Project akhir (company profile)** dibuat setelah UTS dengan 100 kasus yang berbeda.

#### **4. Where (Di mana?)**

- **Lingkungan pengembangan:**
  - **Lokal:** Menggunakan **WSL, VS Code, XAMPP, Postman, Navicat** untuk pengujian awal.
  - **Server:** VPS berbasis **Ubuntu 22 + Apache** untuk meniru lingkungan produksi.
  - **Docker Container:** Menjalankan aplikasi secara terisolasi dalam VPS.

#### **5. Who (Siapa?)**

- **Mahasiswa/Peserta** belajar HTML dan infrastruktur terkait.
- **Instruktur** memberikan materi dan mengawasi proyek.
- **Tim pengembang** (jika ada kerja kelompok) yang berkontribusi dalam proyek akhir.

#### **6. How (Bagaimana?)**

**Langkah-langkah yang dilakukan:**

1. **Persiapan Infrastruktur:**

   - Menyiapkan VPS Ubuntu 22 dengan Apache sebagai server utama.
   - Instalasi dan konfigurasi Docker untuk menjalankan **APP, DB, dan Nginx** dalam container.
   - Menjalankan **XAMPP, VS Code, Postman, Navicat, WSL** di dalam VPS untuk pengelolaan proyek.
2. **Membuat Struktur Folder & File:**

   ```sh
   mkdir pert1
   cd pert1
   mkdir nginx
   touch nginx/nginx.conf
   mkdir src
   touch src/.env
   touch src/docker-compose.yml
   touch src/index.html
   ```
3. **Menulis Konfigurasi Nginx (`nginx.conf`)**

   - Nginx digunakan sebagai proxy untuk mengarahkan traffic ke container yang sesuai.
4. **Membuat File `.env` untuk Konfigurasi Variabel Lingkungan**

   - Menyimpan variabel seperti database credentials, port, dll.
5. **Menulis `docker-compose.yml` untuk Menjalankan Container**

   - Menjalankan **APP, Database (MySQL/PostgreSQL), Nginx** dalam container yang terhubung.
6. **Membuat Halaman Web Dasar (`index.html`)**

   - Menampilkan **header, profile picture, footer dengan social media links** sesuai spesifikasi UTS.
7. **Menggunakan Nginx Proxy Manager & F5.com**

   - Mengelola routing dan domain untuk mempermudah akses website.
8. **Mengerjakan Proyek UTS/UAS (Portfolio & Company Profile)**

   - Membangun website personal untuk UTS/UAS.
   - Mengerjakan **100 kasus unik** dalam proyek akhir berbasis **company profile**.

---

### **2. SWOT ANALYSIS**

| **Faktor**                  | **Analisis**                                                                                                                                                                                                                                                                                                          |
| --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Strengths (Kekuatan)**    | -**Struktur pembelajaran yang jelas** dari dasar hingga proyek nyata. `<br>` - **Menggunakan teknologi modern** seperti Docker, Nginx, dan VPS. `<br>` - **Mendapat pengalaman langsung** dengan manajemen server dan deployment. `<br>` - **Portofolio yang bisa digunakan di dunia kerja**. |
| **Weaknesses (Kelemahan)**  | -**Beban belajar cukup berat** karena banyak teknologi baru yang harus dipahami. `<br>` - **Konfigurasi Docker dan Nginx bisa rumit** bagi pemula. `<br>` - **Manajemen 100 kasus dalam proyek akhir bisa menjadi tantangan** jika tidak ada sistem pengelolaan yang baik.                            |
| **Opportunities (Peluang)** | -**Memahami HTML dasar membuka jalan ke teknologi lain** (CSS, JavaScript, PHP, Laravel, dsb). `<br>` - **Docker & Nginx adalah teknologi industri yang dicari oleh perusahaan**. `<br>` - **Portofolio & company profile bisa digunakan untuk melamar kerja atau proyek freelance**.                 |
| **Threats (Ancaman)**       | -**Kesalahan konfigurasi dapat menyebabkan proyek tidak berjalan dengan baik**. `<br>` - **Kurangnya pemahaman terhadap konsep-konsep dasar bisa menghambat progres**. `<br>` - **Kesulitan dalam mengelola VPS atau sumber daya server yang terbatas**.                                              |

---

### **Kelebihan & Kekurangan Nginx & Docker**

#### **Kelebihan Nginx:**

- Performa tinggi dan ringan dibandingkan Apache.
- Mendukung reverse proxy dan load balancing.
- Stabil dan efisien dalam menangani banyak koneksi simultan.

#### **Kekurangan Nginx:**

- Konfigurasi lebih kompleks dibandingkan Apache.
- Kurang mendukung **modul dinamis** seperti yang ada di Apache.

#### **Kelebihan Docker:**

- Isolasi lingkungan yang baik untuk pengembangan.
- Mempermudah deployment dan reproduksi lingkungan produksi.
- Skalabilitas tinggi dan mendukung **microservices**.

#### **Kekurangan Docker:**

- Konsumsi sumber daya yang tinggi di sistem dengan spesifikasi rendah.
- Kompleksitas dalam manajemen jaringan antar-container.
- Tidak selalu optimal untuk aplikasi dengan **stateful data** tanpa konfigurasi tambahan.

---

### **Kesimpulan**

Dengan pendekatan ini, pembelajaran akan lebih efektif dan proyek akhir bisa diselesaikan dengan baik. 🚀
