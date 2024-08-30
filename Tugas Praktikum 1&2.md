# BAB I PENDAHULUAN 
## 1.1 Latar Belakang
Linux muncul sebagai alternatif yang menarik dibandingkan dengan sistem operasi proprietary seperti Microsoft Windows. Dengan sifat open-source, Linux memberikan kebebasan kepada pengguna untuk mengakses, memodifikasi, dan mendistribusikan perangkat lunak tanpa biaya lisensi yang tinggi. Hal ini menjadi faktor pendorong bagi banyak individu dan organisasi untuk beralih ke Linux, terutama ketika kebijakan pemeriksaan keaslian produk oleh Microsoft semakin ketat.

## 1.2 Tujuan Praktikum
- Memahami Konsep Dasar Sistem Operasi Linux.
- Mempelajari arsitektur dan komponen sistem operasi Linux.
- Mengetahui perbedaan antara Linux dan sistem operasi lainnya seperti Windows dan macOS.

## 1.3 Alat yang digunakan 
1. Laptop.
2. Sistem Operasi Linux/Ubuntu.
3. Virtual Machine/Virtual Box.

# BAB II PEMBAHASAN 
## 2.1 Proses Instalasi 
### Menginstal linux menggunakan Virtual Box
1.	Download Virtual box di web 
2.	Lalu pilih platform packages sesuai laptop anda (Karena Laptop saya memakai Windows jadi saya memilih Windows hosts untuk digunakan)
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(287).png)
3.	Tunggu sampai download an terpasang 
4.	Setelah Virtual Box terpasang lalu buka dan buat project 
5.	Klik new pada virtual box
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(304).png)
6.	Lalu buat project dan sesuaikan seperti nama yang dibutuhkan seperti gambar dibawah ini
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(305).png)
7.	Setelah klik next lalu isi Base Memory sebesar 2048 MB dan menggunakan 2 Processor
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(306).png)
8.	Klik next lagi dan pilih Hard Disk sebesar 20 GB
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(307).png)
9.	Lalu klik Next dan akan menampilkan summary seperti gambar dibawah ini , setelah itu klik finish
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(308).png)
10.	Tampilannya akan seperti gambar dibawah ini jika sudah selesai
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(309).png)
11.	Lalu tambahkan linux Mint pada bagian strorage
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(310).png)
12.	Jika sudah ditambahkan maka tampinnya akan seperti ini
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(311).png)
13. Lalu klik star untuk memulai project
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(312).png)
14. Tunggu Hingga VM nya selesai di buka
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(313).png)
15.	Jika sudah selesai maka tampilan nya akan seperti ini
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshot%20(314).jpeg)
16. Kemudian klik gambar CD dan ikuti langkah-langkah cara pemasangannya seperti gambar di bawah ini
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshoot%20(315).jpeg)
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshoot%20(316).jpeg)
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshoot%20(317).jpeg)
17.	Setelah mengikuti langkah-langkah pemasangan diatas maka tampilannya akan seperti ini
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshoot%20(318).jpeg)
18. Klik Pasang sekarang dan tunggu hingga pemasangan selesai
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/Screenshoot%20(319).jpeg)
19.	Setelah selesai terpasang , Linux pun siap digunakan

## 2.2 Analisis / pada opsi mount point
Partisi “/” dalam sistem operasi Linux memiliki fungsi utama sebagai root directory atau direktori utama. Berikut adalah beberapa fungsi penting dari partisi `/`:
1. Direktori Utama:
   - “/” adalah titik awal dari struktur hierarki direktori Linux. Semua direktori lainnya, seperti “/home”, “/boot”, dan “/usr”, berada di bawah “/”.
2. Instalasi Sistem Operasi:
   - Partisi “/” digunakan untuk menginstal sistem operasi Linux. Semua file sistem operasi, termasuk file konfigurasi, aplikasi, dan data sistem, disimpan di dalam partisi ini.
3. Bootloader:
   - Pada mode UEFI, bootloader diinstal pada partisi dengan label EFI, tetapi partisi “/” harus tetap berada di partisi yang dapat diakses oleh bootloader. Pada mode BIOS, bootloader diinstal di MBR disk, tetapi partisi “/” masih harus berada di partisi yang dapat diakses oleh sistem operasi.
4. Akses dan Akurasi:
   - Pemilihan “/” sebagai mount point memastikan bahwa semua file dan direktori sistem operasi dapat diakses dengan benar. Ini sangat penting karena banyak aplikasi dan skrip yang bergantung pada lokasi “/” untuk berfungsi dengan baik.
5. Konsistensi dan Standar:
   - Menggunakan “/” sebagai mount point mempertahankan konsistensi dengan standar Linux. Hal ini memudahkan pengguna dan pengembang untuk memahami dan bekerja dengan sistem operasi.
     
Dengan demikian, partisi “/” adalah komponen penting dalam sistem operasi Linux yang memungkinkan sistem untuk berjalan dengan stabil dan konsisten dengan standar Linux.

## 2.3 Penjelasan tentang ext4, ext3, swap, ntfs, fat32, dan btrfs
1. ext4 (Fourth Extended File System)
  -	Platform: Linux
  -	Deskripsi: ext4 adalah sistem file yang merupakan evolusi dari ext3. Ini adalah salah satu sistem file default di banyak distribusi Linux modern. ext4 menawarkan perbaikan dalam performa, kapasitas, dan keandalan dibandingkan dengan ext3.
2. ext3 (Third Extended File System)
  -	Platform: Linux
  -	Deskripsi: ext3 adalah sistem file yang digunakan sebelum ext4 dan merupakan evolusi dari ext2. ext3 memperkenalkan fitur journaling yang meningkatkan keandalan sistem file dengan mencatat perubahan sebelum diterapkan.
3. swap
  -	Platform: Linux
  -	Deskripsi: Swap bukanlah sistem file biasa, tetapi sebuah area pada disk yang digunakan sebagai virtual memory untuk memperluas RAM. Jika RAM fisik penuh, data yang tidak aktif dipindahkan ke swap untuk mengosongkan ruang RAM.
4. NTFS (New Technology File System)
  -	Platform: Windows
  -	Deskripsi: NTFS adalah sistem file yang digunakan secara luas di Windows untuk volume dan drive. NTFS mendukung berbagai fitur yang tidak tersedia di FAT32, seperti file permission, enkripsi, dan kompresi.
5. FAT32 (File Allocation Table 32)
  -	Platform: Windows, Linux, macOS
  -	Deskripsi: FAT32 adalah sistem file yang lebih tua dan lebih sederhana dibandingkan NTFS. Meskipun memiliki batasan, FAT32 masih digunakan karena kompatibilitasnya yang luas dengan berbagai sistem operasi dan perangkat.
6. btrfs (B-tree File System)
  -	Platform: Linux
  -	Deskripsi: btrfs adalah sistem file yang dirancang untuk menawarkan fitur-fitur canggih seperti snapshot, subvolume, dan perbaikan integritas data. btrfs masih berkembang dan ditujukan untuk menggantikan ext4 dalam beberapa kasus
