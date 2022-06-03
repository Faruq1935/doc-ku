---
title: "TUGAS 12 BAB-6 KELAS XI TKJ (HAL. 138 SAMPAI DENGAN 153)"
date: 2022-06-03T19:16:34+07:00
draft: false
tags: "Administrasi_Sistem_Jaringan"
---

Kerjakanlah soal esai di bawah ini dengan benar disertai dengan sumber jawabannya!
1. Ada berapa jumlah metode dari prinsip kerja mail server?

   **Jawaban : dua metode**

2. Dalam metode pertama prinsip kerja mail server saat e-mail di kirim, maka e-mail tersebut disimpan pada mail server menjadi satu file berdasarkan tujuan e-mail. File ini berisi informasi sumber dan tujuan, serta dilengkapi ...

   **Jawaban : Tanggal dan waktu pengiriman**

3. Dalam metode pertama prinsip kerja mail server saat user membaca e-mail berarti user telah mengakses server e•mail dan membaca file yang tersimpan dalam server yang ditampilkan melalui … user.

   **Jawaban : Browser**

4. Dalam metode kedua prinsip kerja mail server ketika pengirim mengklik tombol kirim, … memastikan dari ujung ke ujung pengiriman email dari pengirim-sisi server ke server tujuan.

   **Jawaban : SMPTP (MTA)**

5. Dalam metode kedua prinsip kerja mail server setelah mencapai server tujuan, MTA lokal ke server tujuan menerima email, dan dipindahkan ke … setempat. Kemudian menulis email ke kotak pesan penerima.

   **Jawaban : MDA**

6. Dalam metode kedua prinsip kerja mail server ketika penerima memeriksa email, mereka diambil oleh …. dengan menggunakan protokol seperti POP atau IMAP.

   **Jawaban : MUA**

7. webmail hanyalah merupakan frontend dari mail di mana mekanismenya terdapat pada …. dan bukan pada webmail server.

   **Jawaban : Mail Server**

8. Sebutkan perintah yang digunakan untuk install paket-paket mail server di Server Linux Debian!

   **Jawaban : apt install postfix courier-pop courier-imap**

9. Saat instal mail server pada tahapan jendela General Type of mail configuration, yang dipilih adalah ….

   **Jawaban : Internet site**

10. Perintah yang diketikkan di terminal server linux debian untuk membuat directory dari mail yaitu …

    **Jawaban : maildir /etc/skel/maildir**

11. Perintah yang diketikkan di terminal server linux debian untuk meng-edit file main.cf yaitu …

    **Jawaban : nano /etc/postfix/main.cf**

12. Baris text yang ditambahkan dibagian paling bawah dari file main.cf yaitu ….

    **Jawaban : home_mailbox = maildir/**

13. Perintah yang diketikkan di terminal server linux debian untuk re-install postfix seperti pada windows OS tetapi menggunakan konfigurasi yang telah diubah dengan berdasarkan pada konfigurasi sebelumnya yaitu …

    **Jawaban : dpkg-reconfigure postfix**

14. Pada tahapan postfix configuration, yang diisikan pada kotak dialog “system mail name” adalah …

    **Jawaban : mail.nama-user.net**

15. Pada tahapan postfix configuration, saat pengisian kotak dialog “Root and postmaster mail recipient” maka yang perlu dilakukan agar menuju tahapan berikutnya adalah dikosongkan saja, dengan menekan tombol Tab, pada pilihan …. dan akhiri dengan menekan tombol Enter.

    **Jawaban : ok**

16. Pada tahapan postfix configuration, saat pengisian kotak dialog “force synchronous updates on mail queue” yang dipilih adalah …

    **Jawaban : no**

17. Pada tahapan postfix configuration, saat pengisian kotak dialog “local network” ketikkan baris …

    **Jawaban : tambahkan diakhir baris 0.0.0.0/0**

18. Pada tahapan postfix configuration, saat pengisian kotak dialog “use procmail for local delivery “ yang dipilih adalah …

    **Jawaban : no**

19. Pada tahapan postfix configuration, saat pengisian kotak dialog “Internet Protocol to use” agar diarahkan ke versi-4 yang dipilih adalah …

    **Jawaban : ok**

20. Yang perlu ditambahkan baris teks pada file /etc/apache2/apache2.conf dibaris paling bawah yaitu …

    **Jawaban : include "/etc/squirrelmail/apache2.conf"**

21. Yang perlu diubah baris teksnya pada file /etc/squirrelmail/apache.conf di baris #<VirtualHost 1.2.3.4> yaitu ….

    **Jawaban : 
    `<virtualhost *:80>
    DocumentRoot /usr/share/squirrelmail
    ServerName    mail.sudoway.xyz
    </virtualhost>`**

22. Yang perlu diubah baris teksnya pada file /etc/squirrelmail/apache.conf di baris # ServerName webmail.example.com yaitu ….

    **Jawaban : servername mail.thoriq.net**

23. Perintah yang diketikkan di terminal server linux debian untuk membuat user baru dengan nama siswatkj yaitu …

    **Jawaban : adduser junaeditkj**

24. Perintah yang diketikkan di terminal server linux debian untuk me-restart paket courier-imap yaitu …

    **Jawaban : service courier-imap restart**

25. Perintah yang diketikkan di terminal server linux debian untuk me-restart paket courier-pop yaitu …

    **Jawaban : service courier-pop restart**

26. Perintah yang diketikkan di terminal server linux debian untuk me-restart paket postfix yaitu …

    **Jawaban : service postfix restart**

27. Perintah yang diketikkan di terminal server linux debian untuk me-restart paket apache2 yaitu …

    **Jawaban : service apache2 restart "/etc/init.d/apache2 restart"**

28. Setelah berhasil login ke server mail, untuk mulai mengirim pesan email ke pengguna lain, maka yang diklik adalah tombol …

    **Jawaban : menu**

29. Saat akan mengirim email ke pengguna lain, maka perlu mengisi alamat lengkap tujuan di kotak dialog …

    **Jawaban : Cc disi alamat penerima**

30. Saat akan mengirim email ke pengguna lain, maka untuk menentukan judul dari email diketik pada bagian kotak dialog …

    **Jawaban : subjek**

31. Saat akan mengirim email ke pengguna lain, setelah ngisikan dengan lengkap, seperti alamat tujuan email, judul email, dan isi email. Maka tombol yang ditekan agar terkirim ke alamat yang dituju yaitu …

    **Jawaban : send / kirim**

32. Untuk mengecek email yang masuk, maka yang di klik adalah menu …

    **Jawaban : inbox**

33. Untuk mengecek email yang telah terkirim ke pengguna lain, maka yang diklik adalah menu …

    **Jawaban : inbox sent**

34. Untuk mengecek email yang sudah Anda buat akan tetapi belum Anda kirimkan, maka yang diklik adalah menu …

    **Jawaban : inbox drafts**

35. Adalah format iso image yang sering didownload, karena ukurannya yang di bawah 1 GB sehingga akan lebih cepat selesai. Kalimat tersebut merupakan keterangan dari …

    **Jawaban : live cd**

36. Selain bisa dijalankan sebagai live CD alias…. , ternyata beberapa paket instalasi aplikasi populer sudah masuk di dalamnya.

    **Jawaban : tanpa instalasi**

37. Sebutkan beberapa paket instalasi aplikasi populer sudah masuk di dalam LiveCD!

    **Jawaban : file manager, dekstop envirotment contoh XFCE GRNOME KDE, librare office, gimp, web browser contoh firefox biasanya**

38. Dalam LiveDVD, yang membedakannya dengan live CD adalah tentu saja adalah …. yang telah dimuat dalam satu keping DVD.

    **Jawaban : banyaknya software**

39. Dalam LiveDVD hampir seluruh aplikasi populer tersedia bahkan permainan sederhana seperti …

    **Jawaban : mahjong, quadpastell, sudoku**

40. Bin DVD, atau nama lengkapnya adalah binary DVD. Mengapa disebut binary?

    **Jawaban : tidak lain karena anda akan mendapatkan aplikasi deb, rpm package (*.deb, .rpm) dalam keping dvd**

41. MDA kepanjangannya adalah …

    **Jawaban : MDA (Mail Delivery Agent)**

42. POP kepanjangannya adalah …

    **Jawaban : POP3 atau Post Office Protocol**

43. IMAP kepanjangannya adalah …

    **Jawaban :  IMAP atau Internet Message Access.**

44. CMS kepanjangannya adalah …

    **Jawaban : Content Management System**
