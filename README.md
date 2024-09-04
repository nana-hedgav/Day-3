Latihan Hari 3: Aplikasi Todo Sederhana dengan Express
Buatlah aplikasi todo sederhana menggunakan Express yang dapat melakukan operasi berikut:

Membuat todo
Mengupdate todo yang ada
Menghapus todo
Menampilkan daftar todo
Struktur Data Todo
Setiap item todo harus memiliki properti berikut:

id: Pengenal unik untuk setiap todo
description: Deskripsi teks dari todo
date: Tanggal todo dalam format dd-mm-yy
is_checked: Boolean yang menunjukkan apakah todo sudah selesai atau belum
Persyaratan
Buat server Express sederhana yang berjalan di port 3000.

Implementasikan rute-rute berikut:

GET /todos: Menampilkan semua todo
POST /todos: Membuat todo baru
PUT /todos/:id: Mengupdate todo berdasarkan id
DELETE /todos/:id: Menghapus todo berdasarkan id
PATCH /todos/:id/toggle: Mengubah status is_checked todo
Petunjuk Implementasi
Buat fungsi-fungsi terpisah untuk setiap operasi CRUD untuk meningkatkan keterbacaan kode.
Gunakan Date.now().toString() untuk menghasilkan id unik saat membuat todo baru.
Validasi input yang diterima dari klien sebelum menyimpan data.
input dari POST semua harus diisi
input dari PUT hanya boleh mengubah description, date
