# Aplikasi To-Do List Sederhana

## Deskripsi
Aplikasi To-Do List ini memungkinkan pengguna untuk mendaftar dan masuk menggunakan sistem otentikasi berbasis username dan password. Setelah berhasil masuk, pengguna dapat mengakses dan mengelola daftar tugas mereka.

## Fitur
- **Login**: Pengguna dapat masuk menggunakan username dan password yang sudah terdaftar.
- **Sign Up**: Pengguna baru dapat mendaftar dengan memasukkan username dan password.
- **Tampilan Profesional**: Menggunakan desain dengan warna latar belakang gelap untuk kesan profesional.
- **Pengelolaan Pengguna**: Data pengguna disimpan dalam `HashMap` untuk autentikasi login.

## Struktur Kode

### 1. `LoginFrame.java`
- **Fungsi**: Menyediakan antarmuka untuk login pengguna.
- **Komponen Utama**:
  - `JTextField` untuk memasukkan username.
  - `JPasswordField` untuk memasukkan password.
  - Tombol login yang memvalidasi pengguna berdasarkan data yang ada dalam `HashMap`.
- **Logika**:
  - Saat pengguna mengklik tombol login, sistem memeriksa apakah username dan password cocok dengan data yang tersimpan.
  - Jika cocok, pengguna diarahkan ke halaman utama aplikasi.

### 2. `SignUpFrame.java`
- **Fungsi**: Menyediakan antarmuka untuk mendaftar pengguna baru.
- **Komponen Utama**:
  - `JTextField` untuk memasukkan username baru.
  - `JPasswordField` untuk memasukkan password baru.
  - Tombol sign-up untuk mendaftarkan pengguna baru.
- **Logika**:
  - Jika username dan password terisi, data pengguna baru akan disimpan dalam `HashMap` milik `LoginFrame`.
  - Pesan sukses ditampilkan, dan aplikasi akan mengalihkan pengguna ke halaman login.
  - Jika kolom kosong, pesan kesalahan akan ditampilkan.

### 3. Desain Antarmuka
- Menggunakan `GridBagLayout` di `LoginFrame` untuk tata letak responsif.
- Menggunakan layout `null` di `SignUpFrame` untuk penataan manual komponen.

### 4. Pengelolaan Data Pengguna
- Data pengguna (username dan password) disimpan dalam `HashMap` di kelas `LoginFrame`.
- Pengguna yang terdaftar dapat memverifikasi kredensial mereka melalui proses login.

## Cara Menjalankan Aplikasi
1. Pastikan Anda memiliki Java Development Kit (JDK) yang terinstal di sistem Anda.
2. Kompilasi dan jalankan program menggunakan IDE atau terminal.
3. Aplikasi akan membuka jendela login, di mana pengguna dapat memilih untuk mendaftar atau masuk.

## Teknologi yang Digunakan
- **Java Swing**: Untuk membangun antarmuka grafis.
- **Java AWT**: Untuk pengaturan layout dan pengelolaan event.
- **HashMap**: Untuk menyimpan data pengguna sementara.

## Kontribusi
Jika Anda tertarik untuk berkontribusi, silakan buka issue atau buat pull request!

