# Technical Test: Backend Notes Management System
## Tujuan
Membangun aplikasi Notes Management System berbasis REST API yang menerapkan praktik pengembangan backend modern, meliputi authentication, authorization, database design, API architecture, dan deployment.

## Teknologi
### Backend
* Gin **[Nilai Tambah]**, Laravel atau Express
* REST API
* JSON Response

### Database
* MySQL / MariaDB

## Fitur Wajib
### Authentication
* Register
* Login
* Logout
* JWT Authentication

### User Management
* User hanya dapat mengakses data miliknya sendiri

### Notes Management
* Create Note
* Get All Notes (Pagination)
* Get Detail Note
* Update Note
* Delete Note

### Note Attributes
Setiap catatan memiliki:
* Title
* Content
* Status
  * Active
  * Archived
* Created At
* Updated At

### Search & Filter
* Search note berdasarkan title
* Filter berdasarkan status

## Ketentuan Teknis
### API Standards
Menggunakan format response yang konsisten.

Contoh:
```json
{
  "success": true,
  "message": "Note created successfully",
  "data": {}
}
```

### Validation
Minimal validasi:
* Email unik
* Password minimal 8 karakter
* Title wajib diisi
* Content wajib diisi

### Security
* Password wajib di-hash
* Endpoint Notes harus menggunakan JWT Middleware

### Database
Menyediakan file schema .sql berisikan CREATE TABLE untuk tabel yang dibuat

## Nilai Tambah
### Arsitektur
* Layered Architecture / Clean Architecture
* Repository Pattern
* Service Layer

### Dokumentasi
* README.md
* Swagger/OpenAPI
* Postman Collection

### Testing
* Create Note
* Read Note 
* Update Note
* Delete Note

### Deployment
Aplikasi di-deploy dan dapat diakses secara publik.
Contoh:
* Railway
* Render
* VPS
* Docker Container

### DevOps
* Dockerfile
* docker-compose

### Extra Feature
1. Soft Delete Notes
2. Note Categories
3. Note Tags
4. Favorite Notes
5. Activity Log

## Pengumpulan
1. Upload source code ke GitHub (Public).
2. Sertakan README yang berisi:
   * Cara menjalankan aplikasi
   * Struktur project
   * API Documentation
   * URL Deployment
3. Kirim link repository ke [developer@ebyb.com](mailto:developer@ebyb.com) dan WhatsApp HRD

## Deadline
Maksimal 1 Minggu setelah diberikan Test.

## Penilaian
Penilaian akan mempertimbangkan:
* Kecepatan pengerjaan
* Kualitas kode
* Struktur project
* Database design
* API design
* Security
* Dokumentasi
* Deployment
* Commit history
