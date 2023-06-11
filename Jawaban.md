1. Buat direktori dengan nama UAP-Adsis, isi dengan file txt dengan format
penamaan catatannya-<nama kamu>.txt, kemudian isi file txt
tersebut dengan nama dan NIM kamu. Kemudian atur permission
view-only pada file tersebut untuk user biasa. Tunjukkan bukti berupa
screenshot yang menunjukkan bahwa file tersebut berhasil diatur
permissionnya menjadi view-only untuk user biasa.

Jawaban:

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 7.30.04 PM.jpeg">
Membuat folder dan file didalamnya sesuai perintah

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 7.34.45 PM.jpeg">
Menambahkan isi file dengan nim dan nama

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 7.38.46 PM.jpeg">
Mengubah file permission dari user untuk tidak dapat melakukan write

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 7.41.35 PM.jpeg">
Bukti bahwa file sudah tidak dapat di"write"

2. Lakukan konfigurasi alamat IP address sementara pada sistem dan
default gateway. (petunjuk 192.168.56.x | x adalah nomor absen)

Jawaban:

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 7.55.38 PM.jpeg">
Menambahkan ip address untuk ens33 dengan IP 192.168.56.16

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 7.58.32 PM.jpeg">
Menambahkan default gateway dengan command seperti pada image dan mengeceknya


3. Lakukan Instalasi Webmin lalu buatlah user bernama nama anda, lalu
buat group Adsis_(kelas masing-masing) dan masukkan nama anda di
group

Jawaban:

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 9.56.45 PM.jpeg">
Melakukan instalasi webmin sesuai prosedur https://www.digitalocean.com/community/tutorials/how-to-install-webmin-on-ubuntu-22-04

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.04.13 PM.jpeg">
Menambahkan user baru dengan username "adrianaudie"

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.07.36 PM.jpeg">
Membuat group "Adsis_E" dan menambahkan user "adrianaudie" pada group tersebut

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.13.49 PM.jpeg">
<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.15.20 PM.jpeg">
Bukti

4. Lakukan ping ke alamat ip anda dan coba lakukan reject dan drop di
webmin, lalu analisis apa yang terjadi?

Jawaban:

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.20.17 PM.jpeg">
Hasil dari ping ke 192.168.19.128

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.23.51 PM.jpeg">
Menambahkan rule REJECT dan DROP pada paket INPUT melalui Webmin 

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.29.52 PM.jpeg">
Hasil setelah menambahkan rule REJECT dan DROP

5. Buatlah perintah otomatis yang berfungsi untuk ping www.filkom.ub.ac.id

Jawaban:

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.32.56 PM.jpeg">
Menggunakan "crontab -e" untuk mengakses crontab dan melakukan ping otomatis setiap 1 menit

<IMG SRC="/Screenshots/WhatsApp Image 2023-06-11 at 10.36.51 PM.jpeg">
Bukti sistem melakukan ping setiap 1 menit lewat syslog
