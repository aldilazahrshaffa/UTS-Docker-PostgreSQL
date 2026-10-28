
# UTS Docker Compose - PostgreSQL dan pgAdmin

Project ini menggunakan Docker Compose untuk menjalankan PostgreSQL dan pgAdmin.

## Layanan

- **PostgreSQL 15**
  - Port eksternal: 22001
  - Database: postgres
- **pgAdmin 4**
  - Port eksternal: 44001
  - URL: http://localhost:44001

## Persiapan

1. Install Docker Desktop.
2. Salin `.env.example` menjadi `.env`.
3. Sesuaikan isi `.env` dengan konfigurasi yang digunakan.

## Menjalankan Project

Jalankan perintah berikut dari folder project:

```bash
docker compose up -d
```

## Memeriksa Container

```bash
docker compose ps
```

## Menghentikan Container

```bash
docker compose down
```

Data PostgreSQL disimpan dalam Docker volume `postgres_data`.
