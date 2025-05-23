# broadcast-module10

### Experiment 2.1: Original code, and how it run

![Pic1](static/pic1.png)

Saya menjalankan satu server terlebih dahulu dengan perintah cargo run --bin server, lalu buka tiga terminal lain dan jalankan masing-masing client dengan cargo run --bin client. Setelah semua client terhubung, setiap kali salah satu client mengirim pesan, server akan menerima pesan tersebut dan langsung menyebarkannya ke seluruh client yang sedang terhubung, termasuk ke pengirimnya sendiri. Hal ini dimungkinkan karena server menggunakan channel broadcast untuk mengelola semua client yang terkoneksi secara konkuren. Seperti ditunjukkan pada gambar, saat salah satu client mengirim pesan seperti "halo" atau "aku sedang mengerjakan modul 10", semua client lain akan menerima dan menampilkan pesan tersebut, disertai dengan alamat sumber pengirim. Ini membuktikan bahwa sistem broadcast bekerja dengan baik dan bersifat real-time.
