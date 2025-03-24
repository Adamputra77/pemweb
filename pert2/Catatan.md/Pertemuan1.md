Topik hari ini adalah belajar html dasar

Analisa minimal harus ada 5w1h

OS didalam OS

1. Docker : APP, DB,NGINX
2. OS : XAMPP, VSCODE,POSTMAN,NAVICAT,WSL SEMUA MASUK DI VPS -> OS UBUNTU 22 -> APACHE
3. WAJIB : ANALISA, NGODING, CATATAN
4. APA ITU 5W1H -> WHAT,WHY,WHEN

Website

Facebook.com domain

Untuk project uts uas adalah PORTOFOLIO

header,profile picture

footer sosmed semua harus ada di dasbord nya

Project akhir yaitu kasus 100 orang akan mendapatkan kasus yang berbeda2

Project akhirnya Company Profile Sebelum UTS AMBYARRRRRRRRRRRRR

Pembahasan pertemuan kedua adalah HTML itu apa

F5.com Nginx Proxy Manager

kali ini kita membuat pert1 di dalam pert1 ada folder nginx dan didalam folder nginx kita buat file nginx.conf

lalu kita membuat folder src didalam pert1  didalam src ada file .env docker-compose.yml index.html

tag html

p

u

i

b

# Apa itu `tag.html`?

## 1. Jika Maksudnya "Tag dalam HTML"

Dalam HTML, *tag* adalah elemen yang digunakan untuk membangun struktur halaman web. Contoh:

```html
<p>Ini adalah paragraf.</p>
<a href="https://example.com">Ini adalah link.</a>
```

1. HTML
2. CSS
3. INISIALISASI PROJECT
4. BIKIN DB
5. BIKIN MODEL CONTROLER SAMA VIEW
6. BIKIN PROJECT
7. KUMPULKAN PROJECT

lanjut kita buat folder latihan di dalamnya ada home.html dan profile.html


# Langkah-Langkah Membuat `home.html` dan `profile.html`

## 1. Persiapan Folder dan File

1. Buat folder proyek, misalnya `website_project`.
2. Di dalam folder tersebut, buat subfolder `src` untuk menyimpan file HTML.
3. Buat file berikut di dalam `src`:
   - `home.html`
   - `profile.html`
   - `style.css` (untuk menambahkan tampilan yang lebih menarik, opsional).

## 2. Membuat `home.html`

Buat struktur dasar HTML dengan elemen navigasi dan formulir pesan.

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home - Website Saya</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Selamat Datang di Website Saya</h1>
        <nav>
            <ul>
                <li><a href="home.html">Home</a></li>
                <li><a href="profile.html">Profile</a></li>
            </ul>
        </nav>
    </header>

    <section>
        <h2>Tentang Website Ini</h2>
        <p>Website ini dibuat untuk belajar HTML, CSS, dan infrastruktur web.</p>
    </section>

    <section>
        <h2>Hubungi Kami</h2>
        <form action="#" method="post">
            <label for="name">Nama:</label>
            <input type="text" id="name" name="name" required>

            <label for="message">Pesan:</label>
            <textarea id="message" name="message" required></textarea>

            <button type="submit">Kirim</button>
        </form>
    </section>

    <footer>
        <p>© 2025 Website Saya</p>
    </footer>
</body>
</html>
```

3. Membuat profile.html
   Tambahkan informasi dengan  foto dan kontak.

<!DOCTYPE html>

<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile - Adam Putra Pratama</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Profil Saya</h1>
        <nav>
            <ul>
                <li><a href="home.html">Home</a></li>
                <li><a href="profile.html">Profile</a></li>
            </ul>
        </nav>
    </header>

    `<section>`
        `<h2>`Data Diri`</h2>`
        `<p><strong>`Nama:`</strong>` Adam Putra Pratama`</p>`
        `<p><strong>`NIM:`</strong>` 20230801402`</p>`
        `<p><strong>`Prodi:`</strong>` Teknik Informatika`</p>`
    `</section>`

    `<section>`
        `<h2>`Foto Profil`</h2>`
        `<img src="profile.jpg" alt="Foto Profil" width="200">`
    `</section>`

    `<section>`
        `<h2>`Hubungi Saya`</h2>`
        `<p>`Email: `<a href="mailto:adamsap8888@gmail.com">`adamsap8888@gmail.com`</a></p>`
    `</section>`

    `<footer>`
        `<p>`&copy; 2025 Adam Putra Pratama`</p>`
    `</footer>`

</body>
</html>
