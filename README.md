# TUGAS 7

## Penjelasan

- **Stateless Widget** adalah widget yang tidak memiliki data atau keadaan yang bisa berubah selama siklus hidupnya. Contoh: `InfoCard`.
- **Stateful Widget** adalah widget yang memiliki data atau keadaan yang dapat berubah selama siklus hidup widget. Contoh: `MyHomePage`.

### Widget yang Digunakan
1. **AppBar**: Untuk menampilkan header di bagian atas aplikasi.
2. **Scaffold**: Struktur dasar halaman, mencakup `AppBar` dan `body`.
3. **InfoCard**: Kartu yang menampilkan informasi pengguna.
4. **ItemCard**: Kartu dengan ikon dan teks untuk navigasi ke fitur lain.

### Fungsi `setState()`
Digunakan untuk memberitahukan bahwa ada perubahan pada state widget yang perlu di-render ulang.

### Perbedaan `const` dan `final`
- `const`: Nilai harus diketahui pada waktu kompilasi dan tetap sama.
- `final`: Nilai hanya diinisialisasi sekali, tetapi bisa ditentukan pada waktu runtime.

### Implementasi
1. Membuat sebuah app flutter baru
2. Membuah file baru yaitu menu.dart dan diisi sesuai yang dibutuhkan
3. buat 3 button yang bisa dipencet dan harus sesuai tutorial