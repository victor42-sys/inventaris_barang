# Sistem Informasi Inventaris Barang Berbasis Web

## Deskripsi Project

Sistem Informasi Inventaris Barang Berbasis Web merupakan aplikasi yang digunakan untuk mengelola data inventaris secara terstruktur, efisien, dan mudah diakses. Sistem ini membantu admin dalam melakukan pengelolaan data barang dan kategori barang melalui fitur CRUD (Create, Read, Update, Delete), sehingga proses pendataan inventaris menjadi lebih efektif dan terorganisir.

---

## Fitur Utama

1. Login dan Logout Admin menggunakan email dan password.
2. Pengelolaan data barang (tambah, lihat, ubah, dan hapus data barang).
3. Pengelolaan data kategori barang (tambah, lihat, ubah, dan hapus data kategori).
4. Pencarian data inventaris berdasarkan nama barang atau kategori.

---

## Struktur Database

Database terdiri dari tiga tabel utama, yaitu:

### Users

Tabel yang digunakan untuk menyimpan data akun admin yang dapat mengakses sistem.

Field:

- id
- name
- email
- password

### Categories

Tabel yang digunakan untuk menyimpan data kategori barang.

Field:

- id
- category_name
- description

### Items

Tabel yang digunakan untuk menyimpan data inventaris barang.

Field:

- id
- item_code
- item_name
- stock
- condition
- location
- entry_date
- category_id
- user_id

---

## Relasi Database

Relasi antar tabel dalam database adalah sebagai berikut:

- Satu user dapat mengelola banyak data barang.
- Satu kategori dapat memiliki banyak data barang.
- Tabel items terhubung dengan tabel users melalui field user_id sebagai foreign key.
- Tabel items terhubung dengan tabel categories melalui field category_id sebagai foreign key.

---

## Teknologi yang Digunakan

- HTML
- CSS
- JavaScript
- Node.js
- Express.js
- MySQL
- Handlebars (HBS)

---

## Penjelasan Singkat Database

Database terdiri dari tiga tabel utama, yaitu users, categories, dan items.

- users digunakan untuk menyimpan data akun admin yang dapat mengakses sistem.
- categories digunakan untuk menyimpan data kategori barang.
- items digunakan untuk menyimpan data inventaris barang yang dikelola oleh admin.

Hubungan antar tabel memungkinkan setiap barang memiliki kategori tertentu dan tercatat dikelola oleh admin yang melakukan input data. Dengan struktur ini, data inventaris dapat dikelola secara lebih terorganisir dan mudah dicari berdasarkan kategori maupun nama barang.