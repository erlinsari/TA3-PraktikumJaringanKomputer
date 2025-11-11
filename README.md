TUGAS AKHIR Praktikum 3 - Jaringan Komputer E

Nama : Erlin Sari Ramadhani

NPM: 2315061056


Link Youtube : [https://youtu.be/eFliFILn2xw?si=3hFp7rMt88cQZDBu](https://youtu.be/eFliFILn2xw?si=3hFp7rMt88cQZDBu)



Part 1 Build the Network & Basic Configuration
![Part 1 - Build the Network](./screenshots/part1.png)
Pada tahap ini jaringan dibangun dengan dua switch (S1, S2) dan tiga PC (PC-A, PC-B, PC-C). Setelah pemasangan kabel dan console, dilakukan konfigurasi dasar seperti hostname, password, banner, dan IP VLAN 1. Port yang tidak digunakan dimatikan, kemudian IP PC dikonfigurasi sesuai tabel alamat.


Part 2 Create VLANs & Assign Ports
![Part 2 - VLAN Configuration](./screenshots/part2.png)
Tahap ini membuat beberapa VLAN yaitu 10 (Operations), 20 (Parking_Lot), 99 (Management), dan 1000 (Native), serta tambahan 30 (Guest) untuk PC-C. Port-port disesuaikan dengan perangkat, dan IP manajemen dipindahkan ke VLAN 99. Hasil diverifikasi dengan perintah show vlan brief.


Part 3 Maintain VLANs and VLAN Database
![Part 3 - VLAN Maintenance](./screenshots/part3.png)
Pada bagian ini dilakukan percobaan mengubah dan menghapus VLAN. Port diatur ulang menggunakan interface range, dan ketika VLAN dihapus tanpa reassign port, port menjadi tidak aktif. Setelah dikembalikan ke VLAN 1, port kembali berfungsi normal.


Part 4 Configure 802.1Q Trunk
![Part 4 - Trunk Configuration](./screenshots/part4.png)
Port F0/1 pada kedua switch dikonfigurasi menjadi trunk menggunakan Dynamic Trunking Protocol (DTP), lalu diubah ke mode manual dengan switchport mode trunk. Native VLAN juga diubah menjadi 1000 untuk keamanan. Setelah itu, PC-A dan PC-B dapat saling ping antar switch.
