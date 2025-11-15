# NemuKerja — Job Listing & Recruitment Platform

NemuKerja adalah aplikasi web untuk mencari lowongan pekerjaan, melamar, dan mengelola proses rekrutmen.  
Proyek ini dikembangkan sebagai bagian dari mata kuliah **PBL RKS301**.

---

## 🚀 Fitur Utama

- Registrasi & Login pengguna
- Dashboard user & employer
- Posting dan manajemen job listing
- Halaman detail pekerjaan dengan modal dinamis
- Translasi bahasa **EN ↔ ID**
- Sistem pelamaran pekerjaan
- Reset password melalui email
- Alembic migrations untuk sinkronisasi database
- Notifikasi & slot availability system

---

## 🛠️ Teknologi yang Digunakan

- **Python 3**  
- **Flask** (Flask-Login, Flask-Mail, Flask-Migrate, Flask-WTF)  
- **SQLAlchemy**  
- **Alembic** untuk migrasi database  
- **MySQL / phpMyAdmin**  
- **TailwindCSS + Bootstrap 5**  
- **Jinja2 Templates**

---

## ⚡ Cara Instalasi Cepat

> Untuk panduan lengkap dan lebih detail, lihat:  
> 📄 **SETUP_GUIDE.txt**

### 1️⃣ Buat & aktifkan Virtual Environment
```bash
python -m venv .venv
.\.venv\Scripts\activate

### 2️⃣ Install dependencies
pip install -r requirements.txt

### 3️⃣ Atur environment (.flaskenv)
Isi file .flaskenv seperti contoh berikut:
FLASK_APP=run.py
FLASK_DEBUG=1

### 4️⃣ Buat database kosong di phpMyAdmin
Contoh:
nemukerja_db

### 5️⃣ Jalankan migrasi database
flask db upgrade

### 6️⃣ Jalankan aplikasi
flask run --debug

Aplikasi akan berjalan di:
http://127.0.0.1:5000

📦 Struktur Folder
nemukerja/
│── __init__.py
│── models.py
│── forms.py
│── routes/
│── templates/
│── static/
migrations/
run.py
requirements.txt
SETUP_GUIDE.txt
