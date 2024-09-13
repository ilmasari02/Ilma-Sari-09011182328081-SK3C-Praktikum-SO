# LAPORAN
## PRAKTIKUM SISTEM OPERASI
### TUGAS 5

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

## 1.2 Tujuan Praktikum 
- Mengenal konsep proses I/O dan redirection
- Memahami standar input, output dan eror
- Menggunakan notasi output, append dan here document
- Mengenal konsep PIPE dan filter

## 1.3 Alat yang digunakan 
1.Laptop

2.Sistem operasi Linux/Ubuntu

3.Virtual Machine/Virtual Box

# BAB II PEMBAHASAN
## 2.1 Proses Input Output I/O
1. Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke file baru.
![Contoh Gambar]()
2. Lihat daftar secara lengkap pada direktori /etc/paswd, belokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya.
![Contoh Gambar]()
3. Urutkan file baru dengan cara membelokkan standard input.
![Contoh Gambar]()
4. Urutkan file baru dengan cara membelokkan standard input dan standard output ke file baru.urut.
![Contoh Gambar]()
5. Buatlah direktori latihan6 sebanyak 2 kali dan belokkan standard error ke file rmdirerror.txt.
![Contoh Gambar]()
6. Urutkan kalimat berikut:

Jakarta

Bandung Surabaya

Padang

Palembang

Lampung

Dengan menggunakan notasi here document (<@@@...@@@)
![Contoh Gambar]()

7. Hitung jumlah baris, kata dan karakter dari file baru.urut dengan menggunakan filter dan tambahkan data tersebut ke file boru.
![Contoh Gambar]()

8. Gunakan perintah di bawah ini dan perhatikan hasilnya.

$ cat /etc/passwd | sort | pr-n | grep tty03

$find/etc-print | head.

$head/etc/passwd | tail -5 | sort
![Contoh Gambar]()

9. Gunakan perintah $ who | cat | cat | sort | pr | head | cat | tail dan perhatikan hasilnya.
![Contoh Gambar]()

# BAB III PENUTUP 
## 3.1 Kesimpulan
