# Komunikasi Client-Server dengan Enkripsi DES

Proyek ini adalah aplikasi client-server sederhana berbasis Python yang memungkinkan komunikasi terenkripsi menggunakan algoritma DES. Pesan yang dikirim dari client akan dienkripsi atau didekripsi oleh server sesuai mode yang dipilih.

---

## Fitur

- Enkripsi dan dekripsi pesan menggunakan algoritma DES
- Arsitektur client-server sederhana dengan Python socket
- Interaksi berbasis teks
- Mudah dikembangkan (multi-client, GUI, dll.)

---

## Cara Kerja

1. **Client terhubung ke server**
2. **Client mengirim:** mode (`encrypt` atau `decrypt`), pesan, dan kunci
3. **Server memproses permintaan** menggunakan algoritma DES
4. **Server mengirim kembali** hasil enkripsi atau dekripsi ke client

---

Untuk menjalankan simulasi komunikasi saya menggunakan GNS3 dengan menginstall g++. Pada project GNS3 saya membuat topologi sebagai berikut :

<img width="561" alt="image" src="https://github.com/Osvaldo-Kurniawan/Enc_Dcy_Keamanan-Informasi/assets/108170210/425354a2-fa02-4773-bc97-71f1819bd60c">

Dengan catatan ip sebagai berikut :
- ubuntu 1-3 (192.185.1.0) sebagai router penghubung client ke internet (NAT1)
- ubuntu 1-2 (192.185.1.2) sebagai client (menerima input user kemudian melakukan encrypt dan mengirim ke server)
- ubuntu 1-1 (192.185.1.1) sebagai server (menerima pesan client dan melakukan decrypty kemudian menampilkannya)

