# Module 10
##### Deanita Sekar Kinasih
##### 2306229405

## Original code, and how it run
![Image 2.1](images/2_1.png)

Saya menggunakan perintah `cargo run --bin server` untuk menjalankan server dan `cargo run --bin client` untuk menjalankan client. Ketika server dijalankan, muncul pesan "Listening on port 2000" yang menandakan server telah siap menerima koneksi dari client. Setiap kali ada client yang terhubung, server mencatat koneksi baru dengan pesan "New connection from 127.0.0.1:[port]" dengan nomor port yang berbeda-beda. Client yang berhasil terhubung dengan server akan menerima pesan "From server: Welcome to chat! Type a message".
Ketika client pertama mengirim pesan "hello from client 1", server menerima pesan tersebut dan melakukan broadcast ke semua client yang terhubung. Begitu juga ketika client kedua dan ketiga mengirimkan pesan, server akan meneruskan pesan-pesan tersebut ke seluruh client yang terhubung. Dari hasil percobaan terlihat bahwa server berhasil menangani multiple koneksi secara bersamaan dan mendistribusikan pesan dari satu client ke semua client lainnya.