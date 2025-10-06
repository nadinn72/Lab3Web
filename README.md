# Lab3Web

# Langkah Langkah Praktikum

**A. Membuat List di HTML**

*Langkah 1 – Membuat Struktur Awal HTML*

Buat file baru dengan nama lab3_list.html, kemudian isi dengan struktur dasar HTML berikut:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```


<img width="555" height="151" alt="Cuplikan layar 2025-10-06 130411" src="https://github.com/user-attachments/assets/3647d5a7-d20e-471b-8b70-3b7b052e99c8" />



*Langkah 2 – Membuat Ordered List (Daftar Terurut)*

Tambahkan kode berikut di dalam <body>:
```
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>Basis Data 2</li>
    </ol>
</section>
```

<img width="520" height="355" alt="Cuplikan layar 2025-10-06 125628" src="https://github.com/user-attachments/assets/a8b03526-ab72-49cc-ba49-fcb0c247136b" />

Ordered list (OL) digunakan untuk menampilkan daftar yang berurutan dengan angka atau huruf.

*Langkah 3 – Membuat Unordered List (Daftar Tidak Terurut)*

Tambahkan kode berikut di bawahnya:
```
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma & Pemrograman</li>
    </ul>
</section>
```

<img width="793" height="538" alt="Cuplikan layar 2025-10-06 125741" src="https://github.com/user-attachments/assets/5a9a279b-cb64-4e56-8456-e2e7766af812" />

Unordered list (UL) digunakan untuk menampilkan daftar tanpa urutan angka, bisa menggunakan simbol seperti bulat, kotak, atau lingkaran.

*Langkah 4 – Membuat Description List (Daftar Deskripsi)*

Tambahkan kode berikut untuk menampilkan daftar dengan deskripsi:
```
<section id="description-list">
    <h2>Description List</h2>
    <dl>
        <dt>Fakultas Teknik</dt>
        <dd>Teknik Informatika</dd>
        <dd>Teknik Industri</dd>
        <dd>Teknik Lingkungan</dd>
        <dt>Fakultas Ekonomi</dt>
        <dd>Akuntansi</dd>
        <dd>Manajemen</dd>
        <dd>Bisnis Digital</dd>
    </dl>
</section>
```
<img width="1066" height="718" alt="Cuplikan layar 2025-10-06 125943" src="https://github.com/user-attachments/assets/4d444977-0a90-4efb-841d-e6a9365c9f7b" />


**B. Membuat Tabel di HTML**


*Langkah 1 – Membuat Struktur Awal*

Buat file baru bernama lab3_tabel.html dan tambahkan struktur dasar HTML seperti sebelumnya.

*Langkah 2 – Membuat Tabel Sederhana*

Tambahkan kode berikut:
```
<table border="1" cellpadding="4" cellspacing="0">
    <thead>
        <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td>Teknik</td>
            <td>Teknik Informatika</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Teknik</td>
            <td>Teknik Industri</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Teknik</td>
            <td>Teknik Lingkungan</td>
        </tr>
    </tbody>
</table>
```
<img width="726" height="373" alt="Cuplikan layar 2025-10-06 130902" src="https://github.com/user-attachments/assets/1a2fa1bc-8fd6-45c6-9640-bc20dce72ffe" />


*Langkah 3 – Mengatur Padding dan Spasi*

Gunakan atribut cellpadding dan cellspacing untuk mengatur jarak antar sel tabel:
```
<table border="1" cellpadding="6" cellspacing="0">
```

*Langkah 4 – Menggabungkan Sel Data*

Gunakan atribut rowspan dan colspan untuk menggabungkan sel:
```
<td rowspan="3">Teknik</td>
```

<img width="679" height="365" alt="Cuplikan layar 2025-10-06 132000" src="https://github.com/user-attachments/assets/c8cf6f9c-1901-4b88-b97a-192b1dbd03a3" />


**C. Membuat Form (Formulir Web)**


*Langkah 1 – Membuat File Baru*

Buat file baru bernama lab3_form.html.

Tambahkan struktur dasar HTML berikut:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
</body>
</html>
```

*Langkah 2 – Menambahkan Elemen Form*

Tambahkan form sederhana seperti berikut:
```
<form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
        <p>
            <label for="nama">Nama</label>
            <input type="text" id="nama" name="nama">
        </p>
        <p>
            <label for="alamat">Alamat</label>
            <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
        </p>
        <p>
            <label>Jenis Kelamin</label>
            <input id="jk_l" type="radio" name="kelamin" value="L">
            <label for="jk_l">Laki-laki</label>
            <input id="jk_p" type="radio" name="kelamin" value="P">
            <label for="jk_p">Perempuan</label>
        </p>
        <p><input type="submit" value="Kirim"></p>
    </fieldset>
</form>
```
<img width="951" height="379" alt="Cuplikan layar 2025-10-06 132725" src="https://github.com/user-attachments/assets/837acfb8-f159-4fc7-92e3-a4f38889a619" />


*Langkah 3 – Menambahkan CSS untuk Mempercantik Form*

Tambahkan kode CSS di bagian <head>:
```
<style>
    form p > label {
        display: inline-block;
        width: 100px;
    }
    form input[type="text"], form textarea {
        border: 1px solid #197a43;
    }
    form input[type="submit"] {
        border: 1px solid #197a43;
        background-color: #197a43;
        color: #ffffff;
        font-weight: bold;
        padding: 5px 15px;
        border-radius: 5px;
    }
</style>
```

<img width="946" height="378" alt="Cuplikan layar 2025-10-06 133002" src="https://github.com/user-attachments/assets/f1c286a3-18e2-417c-97da-566fbfd5b630" />

