# 🚀 Python MVC Pattern Explorer

## 📋 Tentang Project
Project ini adalah implementasi praktis pola desain Model-View-Controller (MVC) menggunakan Python dan Flask. Dikembangkan sebagai bagian dari kurikulum Software Engineering Academya di Institut Teknologi Bandung (ITB), project ini memberikan pemahaman hands-on tentang konsep MVC dalam pengembangan web.

## 🔍 Apa itu MVC?
MVC (Model-View-Controller) adalah pola arsitektur yang memisahkan aplikasi menjadi tiga komponen utama:
- **Model**: Menangani logika data dan aturan bisnis
- **View**: Menangani tampilan dan presentasi data
- **Controller**: Menangani input pengguna dan menghubungkan Model dan View

## 🛠️ Teknologi yang Digunakan
- Python 3.x
- Flask (Micro web framework)
- SQLAlchemy (ORM untuk database)
- SQLite (Database ringan)

## ⚙️ Persyaratan Sistem
- Python 3.6 atau lebih baru
- pip (Python package installer)
- Terminal atau Command Prompt

## 🚦 Memulai Project

### 1. Clone Repository
```bash
git clone https://github.com/username/mvc-with-python.git
cd mvc-with-python
```

### 2. Setup Virtual Environment (Rekomendasi)
```bash
# Membuat virtual environment
python -m venv venv

# Aktivasi di Windows
venv\Scripts\activate

# Aktivasi di macOS/Linux
source venv/bin/activate
```

### 3. Instalasi Dependencies
```bash
pip install flask flask_sqlalchemy
```

### 4. Jalankan Aplikasi
```bash
python app.py
```
Aplikasi akan berjalan di `http://127.0.0.1:5000/`

## 📝 Pengujian API

### Membuat User Baru
```bash
curl -X POST http://127.0.0.1:5000/users \
  -H "Content-Type: application/json" \
  -d '{"name": "Jane Doe", "email": "jane@example.com"}'
```

### Mendapatkan Semua User
```bash
curl -X GET http://127.0.0.1:5000/users
```

### Mendapatkan User Berdasarkan ID
```bash
curl -X GET http://127.0.0.1:5000/users/1
```

### Memperbarui User
```bash
curl -X PUT http://127.0.0.1:5000/users/1 \
  -H "Content-Type: application/json" \
  -d '{"name": "Jane Updated", "email": "jane.updated@example.com"}'
```

### Menghapus User
```bash
curl -X DELETE http://127.0.0.1:5000/users/1
```

## 📁 Struktur Project
```
mvc-with-python/
├── app.py                 # Entry point aplikasi
├── controllers/           # Direktori controller
│   ├── __init__.py
│   └── user_controller.py # Controller untuk user
├── models/                # Direktori model
│   ├── __init__.py
│   └── user.py            # Model untuk user
├── views/                 # Direktori view (Jika menggunakan template)
├── database.db            # Database SQLite
└── README.md              # Dokumentasi project
```

## 🤝 Kontribusi
Kontribusi selalu diterima! Silakan fork repository ini dan buat pull request untuk mengusulkan perubahan.

## 📜 Lisensi
[MIT License](LICENSE)

## 📧 Kontak
Jika Anda memiliki pertanyaan atau masukan, silakan hubungi [email@example.com](mailto:email@example.com)

---
*Dibuat dengan ❤️ oleh Rivan Permana*
