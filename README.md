# Navigation Flutter

Proyek Flutter ini menunjukkan struktur navigasi sederhana menggunakan named routes. Aplikasi ini terdiri dari tiga layar: first_screen, second_screen, dan third_screen. Pengguna dapat bernavigasi antar layar ini dengan menggunakan tombol dan bottom navigation bar.

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

