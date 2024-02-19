# INSTALASI DEBIAN 12
<br />
<br />

**1. Siapkan Partition di disk**
##
Partition digunakan untuk menyiapkan penyimpanan untuk menyimpan OS Debian, disini saya mengosongkan 40 GB untuk penyimpanan OS Debian saya
![alt](assets/partition.jpg)

##
**2. Masuk ke BIOS Untuk menyeting prioritas boot**
##
Setiap PC memiliki akses ke BIOS seperti di laptop saya menggunakan *F10* untuk masuk ke mode BIOS setelah itu kita atur prioritas boot ke ke USB bootable kita
![alt](assets/bios.jpg)
##
Setelah selesai simpan dan keluar dari mode BIOS, lalu restart PC anda lalu masuk ke instalasi Debian 12

**3. Pilih Bahasa yang digunakan di OS Debian**
##
Disini saya memilih bahasa yang digunakan di OS saya menggunakan bahasa English
![alt](assets/language.jpg)

<br />

**4. Pilih Lokasi Anda**
##
Saya menggunakan Lokasi yang terdekat yang ada di daerah saya
![alt](assets/location.jpg)
<br />
**5. Atur Keymap yang ingin dipakai**
![alt](assets/keymap.jpg)
<br />

**5. Configure Network anda**
##
Configurasi network ini digunakan untuk koneksi untuk menginstalasi debian pada saat installasi debian
![alt](assets/network.jpg)

<br />

**6. Atur Hostname**
##
Pilih Hostname yang ingin anda gunakan
![alt](assets/hostname.jpg)

<br/>

**7. Atur Password yang akan digunakan**
##
Untuk password anda bebas menggunakan apa saja
![alt](assets/password-root.jpg)

<br/>

**8. Mengatur Partition Disk**
##
Kita memecah lagi untuk partition yang di partisi tadi dengan 3 partisi yaitu */ (untuk root)*, */storage (untuk penyimpanan) * dan *swap (untuk swap area)*
![alt](assets/partition-disk.jpg)
<br />
setelah itu change partition yang sudah kita atur
![alt](assets/change-partition.jpg)
<br />

**9. Configure Package Manager**
##
Maksud sini kita mengatur package manager untuk memilih settingan atau template yang digunakan di OS debian 
![alt](assets/configure-pm.jpg)

<br />

**10. Pilih Package Manager yang ada di Indonesia**
##
Disini saya memilih kebo.pens.ac.id 
![alt](assets/idn-pm.jpg)

<br />

**11. Pilih HTTP Proxy**
##
Saya mengosongkan HTTP proxy untuk download Pakcage Manager ini
![alt](assets/http-proxy.jpg)

<br />

**12. Pilih Software yang akan di install dari package kebo**
##
Gunakan settingan default yang ada pada kebo pens
![alt](assets/software-select.jpg)

<br />
Setelah selesai langsung click *continuous* untuk melanjutkan sampai instalasi selesai

##
## Selamat OS Debian dengan Dualboot sudah terinstall di PC anda
<br />
<br />

Artikel ini dibuat untuk memenuhi matakuliah administrasi jaringan yang diampu oleh Bapak Ferry Astika

