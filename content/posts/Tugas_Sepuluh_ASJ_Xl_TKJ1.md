---
title: "Tugas_Sepuluh_ASJ_Xl_TKJ1"
date: 2022-06-03T21:52:16+07:00
draft: false
tags: "Administrasi_Sistem_Jaringan"
---

**Nama : Muhammad Faruq Syarifudin**
**No Nisn : 5925**
**Kelas : Xl TKJ 1**
**Tugas 10 B-6 cara install samba dan quota di debian 8 untuk membatasi penyimpanan setiap user**

Cara install dan konfigurasi file sharing samba dengan quota di Debian 8


Install sistem operasi Debian 11 untuk Sisi server.
Jika sudah selesai lakukan update pada sistem dengan perintah apt update.
Kemudian install paket samba dengan perintah apt install samba.
Setelah selesai lakukan konfigurasi pada file sharing samba dengan perintah                "nano /etc/samba/smb.conf".
Ctrl + w tuliskan read-only kemudian enter setelah itu ubah read-only = yes ke
read-only = no
Kemudian menambahkan user yang berguna untuk client dengan perintah "adduser namauser" Enter terus sampai ada pilihan y/n kemudian pilih y enter.
Kemudian buat password untuk user tersebut dengan perintah "smbpasswd -a namauser" masukaan password yang mudah diingat misal 12345
Setelah itu kita tinggal restart service samba dengan perintah "/etc/init.d/samba restart"
Kita bisa mengecek samba berjalan dengan normal dengan perintah "/etc/init.d/samba status" jika bertuliskan active running berarti konfigurasi berhasil.
Kemudian tambahkan repo nya :
edit source list dengan perinth nano /etc/apt /source.list
# deb-src http://ftp.us.debian.org/debian/ jessie-updates main contrib non-free
# deb-src http://ftp.us.debian.org/debian/ jessie-updates main contrib non-free
seperti biasa setelah update repo haris update “apt update”
Kita langsung ke quota disk dengan perintah "apt install quota" untuk menginstall quota disk pada Debian.
Kemudian kita perlu memperbaharui opsi pemsangan sistem file dengan perintah "nano /etc/fstab"
Akan muncul isi file sebagai berikut :
# /etc/fstab: static file system information.
UUID=06b2aae3-b525-4a4c-9549-0fc6045bd08e	/	ext4	errors=remount-ro	0	1
Kemudian kalian ubah Dan tambahkan seperti berikut :
# /etc/fstab: static file system information.
UUID=06b2aae3-b525-4a4c-9549-0fc6045bd08e	/	ext4	errors=remount-ro,usrquota,grpquota	0	1
Keterangan :
Perubahan di atas akan memungkinkan kita untuk mengaktifkan kuota berbasis pengguna ( usrquota) dan berbasis grup ( ) pada sistem file. grpquota Jika Kalian hanya membutuhkan satu atau yang lain, Kalian dapat mengabaikan opsi yang tidak digunakan.
Pasang kembali sistem file dengan perintah "mount -o remount /".
Kita bisa memverifikasi bahwa opsi baru digunakan untuk memasang sistem file dengan melihat  /proc/mounts file. Di sini, kami menggunakan grepuntuk hanya menampilkan entri sistem file root di file itu : 
cat /proc/mounts | grep ' / '
Hasilnya :
/dev/vda1 / ext4 rw,relatime,quota,usrquota,grpquota,errors=remount-ro,data=ordered 0 0
Ketelah itu ketikan “quotacheck -ugm /”
Lanjutkan dengan “quotaon -v /”
Lanjut dengan menambahkan user baru “adduser namasiswa” enter sampai ada pilihan y/n pilih y
Password samba “smbpasswd -a namasiswa” ketik 123 enter sampai ada pilihan y/n pilih y
Terakhir ketikan “edquota -u namasiswa”
hasilnya : ubah ukuran soft dari 0 ke 102400 lalu juga dengan hard dari 0 ke 102400
Pengujina di lakukan di client windows dengan membuka file manager lalu klik kanan “This Pc” pilih map newtwork ketikan di kolom //192.168.23.2/namasiswa alamat ip tadi dari eth0
masukan user namasisawa dan password 123 klik enter
cobalah untuk mengirim file lebih dari 102400 jika gagal maka anda berhasil :D
coba juga kirim file lebih kecil dari 102400 jika berhasil maka anda dapar nilai dari guru kalian :D
