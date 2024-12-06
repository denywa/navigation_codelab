# Navigation Flutter

Proyek Flutter ini menunjukkan struktur navigasi sederhana menggunakan named routes. Aplikasi ini terdiri dari tiga layar: first_screen, second_screen, dan third_screen. Pengguna dapat bernavigasi antar layar ini dengan menggunakan tombol dan bottom navigation bar.

## Cara Install dan Pakai

### Prasyarat
- Pastikan Anda telah menginstal Flutter SDK di komputer Anda.
- Pastikan Anda memiliki editor kode seperti Android Studio atau Visual Studio Code.

### Langkah-langkah Instalasi
1. Clone repositori ini ke komputer Anda:
   ```bash
   git clone https://github.com/denywa/navigation_codelab.git
   ```
2. Navigasikan ke direktori proyek:
   ```bash
   cd navigation_codelab
   ```
3. Jalankan perintah berikut untuk menginstal dependensi:
   ```bash
   flutter pub get
   ```

### Cara Menjalankan Aplikasi
1. Hubungkan perangkat Android atau iOS Anda, atau siapkan emulator.
2. Jalankan aplikasi dengan perintah berikut:
   ```bash
   flutter run
   ```

## Struktur Proyek

- **lib/main.dart**: Mengatur named routes dan initial route (rute awal).
- **lib/first_screen.dart**: Berisi widget `FirstScreen` dengan navigasi ke Layar Kedua.
- **lib/second_screen.dart**: Berisi widget `SecondScreen` dengan navigasi ke Layar Ketiga.
- **lib/third_screen.dart**: Berisi widget `ThirdScreen` dengan navigasi kembali ke Layar Pertama.

## Fitur

- **Named Routes**: Aplikasi menggunakan rute bernama untuk navigasi, yang diatur pada file `main.dart`.
- **Bottom Navigation Bar**: Setiap layar memiliki bottom navigation bar untuk beralih antar layar.

## Layar

- **first_screen**: Layar awal dengan tombol untuk bernavigasi ke Layar Kedua.
- **second_screen**: Berisi tombol untuk bernavigasi ke Layar Ketiga.
- **third_screen**: Berisi tombol untuk bernavigasi kembali ke Layar Pertama.

## Navigasi

- **first_screen**: 
  - Tombol: Bernavigasi ke Layar Kedua.
  - Bottom NavBar: Memungkinkan beralih ke Layar Kedua dan Ketiga.

- **second_screen**:
  - Tombol: Bernavigasi ke Layar Ketiga.
  - Bottom NavBar: Memungkinkan beralih ke Layar Pertama dan Ketiga.

- **third_screen**:
  - Tombol: Bernavigasi kembali ke Layar Pertama.
  - Bottom NavBar: Memungkinkan beralih ke Layar Pertama dan Kedua.

## Pendekatan dan Tantangan

### Pendekatan
Dalam membangun aplikasi ini, saya memanfaatkan kode yang sudah diberikan di elearn untuk membuat tiap-tiap page dan navigasi antar halaman. selain itu saya juga menambahkan page ketiga dan named routes, saya dapat mengatur semua routesnya di satu tempat, yaitu di `main.dart`. Saya juga menambahkan bottom navigation bar di setiap layar dengan menggunakan logika switch case untuk berpindah halaman.

### Tantangan
Salah satu tantangan yang saya hadapi adalah menentukan `Navigator` yang sesuai untuk digunakan pada tombol third_screen dan bagian bottom navigation bar. Untuk mengatasi ini, saya menggunakan `Navigator.pushNamedAndRemoveUntil` untuk membersihkan stack saat berpindah layar melalui bottom navigation bar. 
