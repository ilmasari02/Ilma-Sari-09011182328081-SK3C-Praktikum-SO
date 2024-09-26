# LAPORAN
## PRAKTIKUM SISTEM OPERASI
### TUGAS 6

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
Konsep job control mulai mendapatkan perhatian yang signifikan pada pertengahan abad ke-20, seiring dengan perkembangan industri dan perubahan dalam organisasi kerja. Pada masa awal industrialisasi, pekerjaan cenderung sangat terstruktur dan monoton, dengan pekerja memiliki sedikit kendali atas proses kerja mereka. Kondisi ini memicu berbagai masalah, seperti penurunan motivasi, produktivitas yang rendah, dan meningkatnya tingkat absensi serta pergantian karyawan.

Para ahli dan praktisi kemudian menyadari bahwa memberikan pekerja lebih banyak otonomi dan kendali atas pekerjaan mereka dapat memberikan manfaat yang signifikan bagi individu dan organisasi. Konsep job enrichment dan job enlargement muncul sebagai upaya untuk meningkatkan kepuasan kerja dan produktivitas dengan memberikan variasi tugas, tanggung jawab yang lebih besar, dan kesempatan untuk mengembangkan keterampilan.

## 1.2 Tujuan Praktikum 
- Mengenal profile
- Mengerti konsep history
- Membuat dan mengeksekusi shell script sederhana
- Mengerti Job control

## 1.3 Alat yang digunakan 
1.Laptop

2.Sistem operasi Linux/Ubuntu

3.Virtual Machine/Virtual Box

# BAB II PEMBAHASAN
## 2.1 Job Control
**1.	Eksekusi seluruh profile yang ada :**
#### a.	Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :
echo “Profile dari /etc/profile”
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(1.a(1)).png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(1.a(2)).png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(1.a(3)).png)

#### b.	Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(1.b(nano%20bash%20%2Clogin%2Cprofile%2Cbashrc)).png)

/home/stD02001/.bash_profile
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(1.b(bash)).png)

/home/. stD02001/.bash_login
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6(1.b(login)).png)

/home/mahasiswa/.profile
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(1.b(profile)).png)

/home/mahasiswa/.bashrc
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(1.b(bashrc)).png)
Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :

echo “Profile dari .bash_profile”

Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.
#### c.	Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:

$ su mahasiswa
$ exit
kemudian gunakan opsi – sebagai berikut :

$ su – mahasiswa
$ exit
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(1.c).png)
Jelaskan perbedaan kedua utilitas tersebut.


**2.	Prompt String (PS)**

#### a.	Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell
PS1=‟> „

export PS1

![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(2.a(1)).png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(2.a(2)).png)

#### b.	Eksperimen hasil PS1 :
$ PS1=“\! > “

69 > PS1=”\d > “

Mon Sep 23 > PS1=”\t > “ 10:10:20 > PS1=”Saya=\u > “

Saya=mahasiswa > PS1=”\w >”

~ > PS1=\h >”
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(2.b).png)

**3.	Logout**

Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout

Echo “Terima kasih atas sesi yang diberikan”
Sleep 5 clear
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(3.(1)).png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(3.(2)).png)

**4. Bash script**
#### a.	Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :
p1.sh

#! /bin/bash

echo “Program p1” 

ls –l

![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(P1))%201.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(P1))%202.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(P1))%203.png)

p2.sh

#! /bin/bash

echo “Program p2” 

who

![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(P2))%201.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(P2))%202.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(P2))%203.png)

p3.sh

#! /bin/bash

echo “Program p3” 

ps x

![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(p3))%201.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(p3))%202.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.a(p3))%203.png)

#### b.	Jalankan script tersebut sebagai berikut :

$ ./p1.sh ; ./p3.sh ; ./p2.sh
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.b)%20perintah%201.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/NOMOR%204.B%20(p1).png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/NOMOR%204.B%20(p3).png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/NOMOR%204.B%20(p2).png)

$ ./p1.sh &
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.b)%20perintah%202.png)

$ ./p1.sh $ ./p2.sh & ./p3.sh &
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/p6%20(4.b)%20perintah%203.png)

$ ( ./p1.sh ; ./p3.sh ) &
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(4.b)%20perintah%204.png)

**5.	Jobs**
#### a.	Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.

#!/bin/bash 

while [ true ] 

do

date >> hasil 

sleep 10

done

![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(5.a)%201.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(5.a)%202.png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(5.a)%203.png)

#### b.	Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :
$ jobs

$ find / -print > files 2>/dev/null &

$ jobs
#### c.	Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background
$ fg %1

$ bg
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(5.b.c).png)

#### d.	Stop program background dengan utilitas kil

$ ps x
$ kill [Nomor PID]
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(5.d%20)%201.png)

**6.	History**
#### a.	Ganti nilai HISTSIZE dari 1000 menjadi 20
$ HISTSIZE=20
$ h
#### b.	Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan
$ !-5
#### c.	Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer
$ !!
#### d.	Ulangi instruksi pada history bufer nomor 150
$ !150
#### e.	Ulangi instruksi dengan prefix “ls”
$ !ls
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(6).png)
![Contoh Gambar](https://github.com/ilmasari02/Ilma-sari-09011182328081-SK3C-Praktikum-SO/blob/main/Sistem%20Operasi/P6%20(6.1).png)

# BAB III PENUTUP 
## 3.1 Kesimpulan


