## MEMBUAT APLIKASI JASA LAUNDRY ( S B L ) <br>
## 1.1 Latar Belakang
  Kemajuan teknologi informasi yang sangat cepat dan memasuki ke seluruh sektor dalam kehidupan sangat memungkinkan siapa saja dan apa saja yang sebelumnya tidak terbayangkan menjadi sebuah kenyataan. 
  Termasuk lingkungan pesantren, tempat lembaga pendidikan keagamaan yang masih eksis hingga saat ini, digitalisasi di dalam Pondok Pesantren menjadi salah satu tanda bahwa lembaga pesantren bukan lembaga pendidikan yang kurang menerima akan kemajuan dalam bidang teknologi informasi. 
  kali ini saya mengambil studi kasus dari pondok pesantren, yakni dengan membuat sistem layanan laundry digital dimana mempermudah  santri dalam melakukan pendataan, penjadwalan dan berbagai macam fitur yang dapat mempermudah  dalam  bidang jasa laundry pondok. <br>
  
  ## 1.2 Deskripsi Teknologi Informasi
Aplikasi Jasa LAundry ini diberi nama S B L, singkatan dari Sumur Bandung Laundry. Aplikasi yang bergerak di dalam jasa Laundry. Aplikasi ini dapat : <br>
1. Memesan Laundry dengan mudah dan simpel. <br>
2. Menerima Notifikasi Pengingat Jadwal Laundry <br>
3. Mengatur limit pemesanan Laundry dalam se bulan.  <br>
  

  ## 1.3 Branding 
 Adapun Brand yang dirancang dalam sistem aplikasi laundry ini adalah : <br>

Merk: S B L <br>
Tagline: Laundry Mundah !<br>
Campaign: Bagaimana membuat aplikasi yang memperrmudah sistem layanan Laundry di " Pondok Pesantren Pembangunan Sumur Bandung "<br>
Target user:<br>
Santri aktif "Pondok Pesantren Pembangunan Sumur Bandung".<br>
User experience theme:<br>
Sederhana,
Mudah<br>
Warna: Dominan Hijau, Sesuai dengan warna dominan Pondok <br>
Design : <br>


![Deskripsi Gambar](design.png)


  ## 2. User Story
  Sebagai | Saya Ingin | Supaya Dapat | Prioritas
---|---|---|---
Pengguna | Memesan Pesanan | Mendapatkan jasa layanan yang diingikan dalam memesan pesanan | ⭐⭐⭐⭐⭐
| | |
Pengguna | Mendapat notifikasi pengingat | Dapat teringat jadwal Laundry User | ⭐⭐⭐⭐
| | |
Pengguna | Memesan sesuai kategori | Memesan Per kategori Laundry | ⭐⭐⭐⭐⭐
| | |
Pengguna | Melihat Jadwal dan Riwayat Laundry | Mengetahui jadwal Laundry ayng belum terlaksana, beserta riwayat Laundry yang sudah selesai | ⭐⭐⭐⭐

## 3. Struktur Data
```mermaid
erDiagram
    PENGGUNA ||--o{ LAYANAN  : memesan
    PENGGUNA {
        int nomor_induk_santri
        string NAMA
        string divisi_sekolah
        string password
    }
    LAYANAN ||--|{ LINE-ITEM : mengandung
    LAYANAN {
        string Layanan_Jasa
        string jenis_layanan
        string jumlah_pesanan
    }
    LINE-ITEM {
        int Nomor_pesanan
        string Jadwal_laundry
        float Limit_laundry
    }
```
## 4. Arsitektur Sistem
```mermaid
flowchart TD
    Database:Firebase <--> Aplikasi_Web_Backend:JavaScript-express.js <--> Web_server:JavaScript-express.js <--> Aplikasi_AndroidDan_IOS:Flutter_Dart
```
## 5. Teknologi, Library, dan Framework

## 6. Desain User Experience dan User Interface
! [Link](https://www.figma.com/proto/fyEcP3JXW92TcKZXS8RXFH/SB-Laundry?page-id=0%3A1&type=design&node-id=34-37&t=IFAAdm7krjaNnifP-1&scaling=scale-down&starting-point-node-id=0%3A3&mode=design)

## 7. Demonstrasi Video
## 8. Dalam video, jelaskan bagaimana mesin komputasi dan sistem operasi berperan dalam produk teknologi informasimu !
## 9. Dalam video, jelaskan bagaimana algoritma, struktur data, dan bahasa pemrograman berperan dalam produk teknologi informasimu !
## 10. Dalam video, jelaskan bagaimana metode pengembangan perangkat lunak / Software Development Life Cycle berperan dalam produk teknologi informasimu !
## 11. Dalam video, jelaskan bagaimana database / sistem basis data berperan dalam produk teknologi informasimu !


