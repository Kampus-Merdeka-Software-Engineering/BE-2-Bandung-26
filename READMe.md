# Backend Naratif Indonesia

Naratif Indonesia adalah portal berita digital yang didirikan pada tahun 2023.

Portal berita ini berfokus pada penyediaan berita dan analisis mendalam dari berbagai bidang, termasuk politik, ekonomi, sosial, budaya, dan teknologi dengan Developer Group 26.

Readme.md pada halaman ini terkait Backend yang dibangun menggunakan teknologi Node.js, Express, dan database MySQL dengan menggunakan Railway.

## Instalasi

Untuk menjalankan backend ini, pastikan sudah melakukan instalasi package dengan menggunakan NPM.

Instal package.json, gunakan perintah:

```bash
  npm init -y
```

Install nodemon, gunakan perintah:

```bash
  npm i nodemon --save-dev
```

Install dotenv, cors, express, dan mysql2, gunakan perintah:

```bash
  npm i dotenv cors express mysql2
```

## Struktur Folder

- config: Berisi konfigurasi aplikasi termasuk
- pengaturan koneksi ke database.
- helper: Berisi fungsi bantuan yang digunakan di - berbagai bagian aplikasi.
- service: Berisi logika bisnis dan interaksi dengan database.
- routes: Berisi endpoint-endpoint API yang tersedia.


## Cara Menjalankan

Untuk menjalankan server, gunakan perintah:

```bash
  npm run dev
```
    
## API Reference

```http
https://be-2-bandung-26-production.up.railway.app/berita
```

#### Get all berita

```http
GET /berita
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `page` | `number` | Page number for pagination |

#### Get a specific berita

```http
GET /berita/${id}

```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. ID of the news item |

#### Get berita by topic

```http
GET /berita/topik/${topik}

```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `topik`      | `string` | **Required**. News topic |




