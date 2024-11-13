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

# TUGAS 8

### Apa kegunaan const di Flutter? Jelaskan apa keuntungan ketika menggunakan const pada kode Flutter. Kapan sebaiknya kita menggunakan const, dan kapan sebaiknya tidak digunakan?
const digunakan untuk membuat nilai yang tetap (konstan) pada saat kompilasi. Dengan menggunakan const, Flutter akan membuat objek hanya sekali di memori dan menggunakannya kembali jika objek yang sama dibutuhkan. Keuntungan menggunakan const adalah mengurangi penggunaan memori dan meningkatkan performa aplikasi karena objek yang sama tidak perlu dibuat berulang kali.

### Jelaskan dan bandingkan penggunaan Column dan Row pada Flutter. Berikan contoh implementasi dari masing-masing layout widget ini!
Secara singkat`column` digunakan untuk menyusun widget kebawah (vertikal) dan `row` untuk menyusun widget ke samping (horizontal)

```dart
Column(
  children: [
    Text("Widget 1"),
    Text("Widget 2"),
    Text("Widget 3"),
  ],
)
```

```dart
Column(
  children: [
    Text("Widget 1"),
    Text("Widget 2"),
    Text("Widget 3"),
  ],
)
```

```dart
Row(
    mainAxisAlignment: MainAxisAlignment.spaceEvenly,
    children: [
    InfoCard(title: 'NPM', content: npm),
    InfoCard(title: 'Name', content: name),
    InfoCard(title: 'Class', content: className),
    ],
),
```

### Sebutkan apa saja elemen input yang kamu gunakan pada halaman form yang kamu buat pada tugas kali ini. Apakah terdapat elemen input Flutter lain yang tidak kamu gunakan pada tugas ini? Jelaskan!
Pada tugas kali ini saya hanya menggunakan TextFormField untuk input name, amount, dan description. 

### Bagaimana cara kamu mengatur tema (theme) dalam aplikasi Flutter agar aplikasi yang dibuat konsisten? Apakah kamu mengimplementasikan tema pada aplikasi yang kamu buat?
Tema dapat diatur di main.dart di MaterialApp menggunakan ThemeData. Dalam tugas ini saya menggunakannya untuk mengatur warna.

### Bagaimana cara kamu menangani navigasi dalam aplikasi dengan banyak halaman pada Flutter?
Navigasi dalam aplikasi dengan banyak halaman pada Flutter dapat ditangani dengan menggunakan Navigator. Navigator digunakan untuk mengelola tumpukan halaman (routes) dalam aplikasi Flutter. Navigator memiliki method untuk menampilkan halaman baru, menghapus halaman, dan kembali ke halaman sebelumnya. Navigasi dapat dilakukan dengan menggunakan Navigator.push() untuk menampilkan halaman baru dan Navigator.pop() untuk kembali ke halaman sebelumnya.