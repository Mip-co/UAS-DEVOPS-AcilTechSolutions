# UAS DevOps - AcilTech Solutions

## 📖 Tentang Proyek

Proyek ini dibuat sebagai tugas Ujian Akhir Semester (UAS) mata kuliah DevOps.

Tujuan utama dari proyek ini bukan hanya membuat sebuah website sederhana, tetapi juga mempelajari proses deployment dan otomatisasi menggunakan konsep CI/CD dengan lingkungan self-hosted.

---

## 🎯 Tujuan Proyek

- Mempelajari dasar konsep DevOps.
- Mengimplementasikan CI/CD menggunakan GitHub Actions.
- Melakukan deployment website pada server Linux.
- Menggunakan Nginx sebagai web server.
- Menggunakan Cloudflare Tunnel untuk publikasi website.
- Memahami dasar pengelolaan infrastruktur server.

---

## 🛠️ Teknologi yang Digunakan

### Frontend

- HTML
- CSS

### Infrastruktur

- Ubuntu Server
- Nginx
- GitHub Actions
- Self-hosted Runner
- Cloudflare Tunnel

### Tools

- Git
- GitHub

---

## 🚀 Alur Deployment

```text
Developer
     │
     ▼
Git Push (branch main)
     │
     ▼
GitHub Actions
     │
     ▼
Self-hosted Runner
     │
     ▼
Menghapus file lama
     │
     ▼
Menyalin file terbaru
     │
     ▼
Reload Nginx
     │
     ▼
Cloudflare Tunnel
     │
     ▼
Pengguna
```

---

## ⚙️ Cara Kerja CI/CD

Ketika terdapat perubahan kode yang di-push ke branch `main`, maka:

1. GitHub Actions akan berjalan secara otomatis.
2. Self-hosted runner menjalankan workflow deployment.
3. File website lama akan diganti dengan file terbaru.
4. Service Nginx akan di-reload.
5. Website dapat diakses melalui Cloudflare Tunnel.

---

## ⚠️ Kendala yang Dihadapi

Selama pengerjaan proyek terdapat beberapa kendala, di antaranya:

- Keterbatasan biaya untuk menyewa VPS.
- Implementasi Docker yang belum berhasil diterapkan.
- Menyesuaikan deployment dengan lingkungan self-hosted.

Untuk mengatasi hal tersebut, dipilih solusi menggunakan Linux VM, Cloudflare Tunnel, dan GitHub Actions.

---

## 💡 Alasan Menggunakan Cloudflare Tunnel

Pada proyek ini Cloudflare Tunnel dipilih karena:

- Lebih hemat biaya.
- Tidak perlu menyewa VPS.
- Mudah dikonfigurasi.
- Cocok untuk kebutuhan pembelajaran dan proyek mahasiswa.

---

## 📂 Struktur Repository

```
.
├── .github/
│   └── workflows/
├── assets/
├── index.html
└── README.md
```

---

## 👨‍💻 Peran Saya

Pada proyek ini saya bertanggung jawab dalam:

- Konfigurasi deployment
- Pembuatan workflow GitHub Actions
- Konfigurasi Self-hosted Runner
- Konfigurasi Nginx
- Konfigurasi Cloudflare Tunnel
- Pengelolaan server Linux dasar

---

## 📚 Hal yang Dipelajari

Melalui proyek ini saya mempelajari:

- Dasar CI/CD
- Manajemen service Linux
- GitHub Actions
- Konfigurasi Nginx
- Deployment menggunakan Self-hosted Runner
- Dasar otomatisasi infrastruktur
- Troubleshooting deployment

---

## 🚧 Pengembangan Selanjutnya

Beberapa hal yang ingin dikembangkan pada proyek ini:

- Implementasi Docker
- Monitoring dan logging
- Peningkatan keamanan server
- Optimasi deployment
- Penggunaan reverse proxy yang lebih baik

---

## 📝 Catatan

Repository ini dibuat untuk keperluan pembelajaran dan tugas UAS mata kuliah DevOps.
