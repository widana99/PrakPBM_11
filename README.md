# Aplikasi CRUD Mahasiswa dengan Login - Flutter + SQLite
---
Aplikasi Flutter ini merupakan aplikasi CRUD (Create, Read, Update, Delete) sederhana untuk mengelola data mahasiswa, dengan sistem login admin dan penyimpanan data menggunakan SQLite lokal.

# Fitur Aplikasi
---
- ### Login Admin
    - Akses aplikasi hanya oleh admin dengan username dan password yang telah ditentukan.
    - Username default: admin
    - Password default: password
- ### Manajemen Data Mahasiswa
    - Tambah data mahasiswa baru.
    - Lihat daftar seluruh mahasiswa.
    - Edit data mahasiswa.
    - Hapus data mahasiswa.
- ### Logout
    - Keluar dari halaman utama kembali ke halaman login.

# Screenshot
---
## Halaman Awal
![image](https://github.com/user-attachments/assets/75a9a11c-b225-4c0b-bdc6-389589cfcc0c)
---
## Halaman Isi
![image](https://github.com/user-attachments/assets/73a95198-9132-4f64-aab6-51ee1338b63e)
![image](https://github.com/user-attachments/assets/6d204c86-9efb-4433-abb4-d6e741a4dad1)
![image](https://github.com/user-attachments/assets/b4a6d2f3-54f3-462a-bb72-746d5f29e36d)
---
# Alur Program
---
1. ### LoginPage
    - Halaman awal untuk login.
    - Hanya admin yang dapat mengakses aplikasi.
2. ### MainPage
    - Menampilkan daftar mahasiswa dari database lokal.
    - Terdapat tombol:
       - Tambah mahasiswa baru
       - Edit data mahasiswa
       - Hapus mahasiswa
       - Logout kembali ke LoginPage
3. ### StudentFormPage
     - Form input untuk menambah atau mengedit data mahasiswa.
4. ### DatabaseHelper
     - Singleton class untuk mengelola database SQLite:
        - Membuat tabel jika belum ada.
        - Menyimpan data mahasiswa.
        - Mengambil data mahasiswa.
        - Memperbarui data mahasiswa.
        - Menghapus data mahasiswa.
