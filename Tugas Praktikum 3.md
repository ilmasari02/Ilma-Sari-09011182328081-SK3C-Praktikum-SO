# LAPORAN
## PRAKTIKUM SISTEM OPERASI
### TUGAS 3

---

### Disusun oleh:
**Nama**: Ilma Sari

**NIM** : 09011182328081

**Kelas** : SK3C

**Dosen Pengampu** :Adi Hermansyah, M.T.

---

### PROGRAM STUDI SISTEM KOMPUTER 
### FAKULTAS ILMU KOMPUTER 
### UNIVERSITAS SRIWIJAYA
**2024**

# BAB I PENDAHULUAN
## 1.1 Latar Belakang
Dalam era digital saat ini , kemampuan mengelola server dan sistem operasi berbasis teks menjadi semakin penting. Praktikum command line ini bertujuan untuk memberikan pemahaman dasar tentang penggunaan command line pada sistem operasi Linux, yang banyak digunakan dalam lingkungan server.
## 1.2 Tujuan Praktikum 
- Mampu mengakses dan mengelola sistem file linux menggunakan perintah-perintah dasar
- Mampu menginstal dan mengkonfigurasikan perangkat lunak menggunakan manager paket
- Memahami dasar-dasar scripting sheel untuk otomatisasi tugas 

## 1.3 Alat yang digunakan 
1.Laptop

2.Sistem operasi Linux/Ubuntu

3.Virtual Machine/Virtual Box

# BAB II PEMBAHASAN
## 2.1 Membuat 50 Command Line 
1. uname : Menampilkan informasi tentang sistem operasi
2. lscpu : Menampilkan informasi tentang CPU
   ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%201%262.png)
3. lsblk : Menampilkan informasi tentang perangkat blok
4. df -h : Menampilkan penggunaan disk dalam unit human-readable (MB, GB,dll.)
5. free -m : Menampilkan penggunaan memori dalam megabyte
6. pwd : Menampilkan direktori kerja saat ini
7. ls : Menampilkan daftar file dan direktori kerja saat ini
8. touch ilma123 : Membuat file kosong bernama "ilma123"
9. ls : Menampilkan file "ilma123"
10. rm ilma123 : Menghapus file "ilma123"
11. ls : Menampilkan file yang sudah terhapus "ilma123"
   ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%203-9.png)
12. mkdir ilma123 :Membuat directori bernama "ilma123"
13. ls : Menampilkan file "ilma123"
14. rm -rf ilma : Menghapus secara permanent directori "ilma123" tanpa meminta konfirmasi
15. ls : Menampilkan file yang sudah terhapus "ilma123"
16. du : Menampilkan ukuran disk yang digunakan oleh file dan directori
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%2010-16.png)
17. useradd : Menambahkan pengguna batu
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%2017.png)
18. userdel : Menghapus pengguna 
19. awk : bahasa pemrograman untuk memproses data teks
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%2018-19.png)
20. date : menampilkan tanggal dan waktu saat ini 
21. zsh : shell yang lebih interaktif dengan fitur pelengkapan otomatis yang kuat 
22. bush : shell default di banyak sistem Linux 
23. fish : shell yang dirancang untuk pengguna baru dengan sintaks yang sederhana 
24. history : Menampilkan daftar perintah yang pernah dijalankan 
25. man : Menampilkan manual halaman untuk suatu perintah 
26. which : Mencari lokasi sebuah program 
27. whereis : Mencari lokasi biner,sumber,dan manual halaman dari sebuah perintah
28. locate : Mencari file berdasarkan nama (perlu database yang diperbarui)
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%2020-28.png)
29. chmod : Mengubah izin akses 
30. hostname : Menampilkan nama host
31. whoami : Menampilkan nama pengguna saat ini  
32. cal : Menampilkan kalender
33. ps aux : Menampilkan semua proses yang sedang berjalan 
   ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%2029-33.png)
34. top : Menampilkan informasi real-time tentang penggunaan sistem
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%2034.png)
35. python script.py : Menjalankan skrip Python bernama script.py
36. gcc program.c -o program : Mengkompilasi program C menjadi program yang dapat dieksekusi
37. systemctl start apache2 : Memulai layanan Apache (web server) pada sistem berbasis Debian/Ubuntu
38. grep "pola" file : Mencari baris yang mengandung pola tertentu dalam sebuah file 
39. sudo apt update : Memperbarui daftar paket
40. sudo apt install word : Menginstal word
41. sudo apt remove word : Menghapus word 
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%2035-42.png)
42. kill PID : Mengakhiri proses dengan ID tertentu
43. ping alamat IP : Mengirim paket ICMP ke alamat IP untuk menguji konektivitas 
44. unzip arsip.zip : Mengekstrak isi arsip zip
45. du -sh : Menampilkan ukuran disk yang digunakan oleh file dan direktori
46. netstat -a: Menampilkan semua koneksi TCP dan UDP, baik yang aktif mqaupun yang sedang mendengarkan 
    ![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/command%2043-47.png)
47. netstat -tunp : Menampilkan koneksi TCP dan UDP yang sedang mendengarkan, beserta proses yang terkait
48. rm -i file_berbahaya : Menghapus file secara interaktif, meminta konfirmasi sebelum menghapus 
49. sed 's/old/new/g' file : Mengganti teks dalam sebuah file
50. shutdown : Mematikan atau me-restart sistem
    ![Contoh Gambar](

# BAB III PENUTUP 

    















