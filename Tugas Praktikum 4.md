# LAPORAN
## PRAKTIKUM SISTEM OPERASI
### TUGAS 4

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
Sistem operasi Linux dikenal dengan fleksibilitas dan kemampuan kustomisasi yang tinggi, salah satunya dalam pengelolaan sistem file. Pemahaman yang mendalam tentang struktur direktori, izin akses, dan berbagai jenis link sangat krusial bagi pengguna Linux, baik untuk pengguna biasa maupun administrator sistem.

## 1.2 Tujuan Praktikum 
- Mengenal organisasi File di Linux
- Menciptakan dan memanipulasi direktori
- Mempelajari ijin akses (permission) dari file dan direktori
- Mengenal konsep Owner dan Group
- Mengerti konsep Linux dan symbolic link

## 1.3 Alat yang digunakan 
1.Laptop

2.Sistem operasi Linux/Ubuntu

3.Virtual Machine/Virtual Box

# BAB II PEMBAHASAN
## 2.1 Sistem File (File System)
1. Lihat peralatan I/O, character device, yang ada pada system komputer.
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(1).png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(1.1).png)
2. Buatlah sub direktori **januari, februari** dan **maret** sekaligus pada direktori **latihan5**.
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(2).png)
3. Buatlah file dataku yang berisi **nama, nim** dan **alamat** anda pada sub direktori **januari** dan copy-kan file tersebut ke sub direktori **februari** dan **maret**.
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(3).png)
4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga **group** dan others dapat melakukan **write**.
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(4).png)
5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat melakukan baik **write, read** maupun **execute**, tetapi group dan others hanya bisa read dan execute.
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(5).png)
6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan **write, read** dan **execute**.
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(6).png)
7. Hapuslah direktori **maret**.
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(7).png)
8. Ubahkan kepemilikan sub direktori **februari** sehingga **user** dan **group** hanya dapat melakukan **read**, dan cobalah untuk membuat direktori baru **haha** pada sub direktori **februari**.
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(8).png)
9. Modifikasi **umask** dari file dataku pada sub direktori **januari** menjadi **027** dan berapakan nilai default-nya?
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(9).png)
10. Buatlah **link** dari file dataku ke file **dataku.ini** dan file **dataku.juga** dan dengan perintah **list** perhatikan berapa **link** yang terjadi?
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/praktikum4%20(10).png)

# BAB III PENUTUP 
## 3.1 Kesimpulan
Melalui praktikum ini, dapat disimpulkan bahwa sistem file Linux memiliki struktur yang hierarkis dan fleksibel. Perintah-perintah seperti mkdir, cp, chmod, chown, dan ln merupakan alat yang sangat berguna untuk memanipulasi direktori dan file. Konsep izin akses, kepemilikan, dan jenis link sangat penting untuk menjaga keamanan dan integritas sistem file.

Pengaturan izin akses yang tepat akan mencegah akses yang tidak sah ke data sensitif. Pemahaman tentang hard link dan symbolic link memungkinkan pengguna untuk membuat berbagai jenis referensi ke file yang sama. Sementara itu, umask memberikan cara yang mudah untuk mengatur izin default untuk file yang baru dibuat.
