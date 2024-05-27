```
{
    Nama    : Agung Dwi Nugroho
    NRP     : 3122600006
    Kelas   : 2 STr IT A
}
```

# Instalasi Debian Menggunakan VirtualBox

### Setup Oracle VM VirtualBox
**1. Main Screen**<br>
![homescreen virtualbox](./assets/1.png)<br>
Untuk menambahkan machine baru, klik pada new yang terletak di main screen virtualbox.
<br>
**2. Nama VM dan OS**<br>
![Nama VM dan OS](./assets/2.png)<br>
Akan muncul screen untuk mengatur nama machine dan image dari OS yang akan digunakan. Sesuai penugasan, nama dari machine adalah 'SysAdmin-NRP'. Selain itu, saya menyimpan machine ini di direktori `D:\VM\Deb` dan menggunakan image Debian 12 yang terdapat pada direktori `D:\Downloads\`. Pastikan mencentang checkbox *skip unanttended installation* supaya dapat melakukan setup Debian secara manual nantinya.
<br>
**3. Hardware Spec**<br>
![Hardware](./assets/3.png)<br>
Setelah setup VM dan OS adalah alokasi spesifikasi hardware yg digunakan. Saya menggunakan 4 GB memori dan 2 Core CPU.
<br>
**4. Storage**<br>
![Storage](./assets/4.png)<br>
Selanjutnya adalah membuat virtual hard disk. Sesuai dengan penugasan, kapasitas hard disk yang dipakai adalah 25 GB.
<br>
**5. Summary**<br>
![Summary](./assets/5.png)<br>
Jika semua sudah selesai, maka bisa lanjut finish.
![Result](./assets/6.png)<br>
Dan virtual machine akan muncul di halaman utama Virtualbox. Selanjutnya adalah klik Start pada virtual machine untuk lanjut setup OS.
<br>

### Setup Debian 12
**1. Konfigurasi Network**<br>
- ![hostname](./assets/8.png)
Pertama adalah mengisikan hostname, disini saya isikan sesuai dengan nama virtual machine yakni 'SysAdmin-NRP'.

- ![domain](./assets/9.png)<br>
Selanjutnya untuk domain nama saya isikan default.
<br>
**2. User dan Password**<br>
- ![admin password](./assets/10.png)
Untuk root password saya isikan sebagai 'admin'.

- ![Fullname](./assets/11.png)
Fullname user saya isikan sesuai dengan nama virtual machine.

- ![username](./assets/12.png)
Selanjutnya untuk username saya sesuaikan dengan 

- ![user password](./assets/13.png)
Begitu juga dengan user password saya isikan sebagai 'admin'.
<br>
**3. Partition Disk**<br>
- ![partition method](./assets/14.png)
Pilih metode partisi manual untuk mengatur alokasi sesuai dengan penugasan.

- ![config](./assets/15.png)
Pilih disk sesuai dengan kapasitas yg telah dibuat sebelumnya.

- ![config](./assets/16.png)
Arahkan pada partisi FREE SPACE.

- ![root partition](./assets/18.png)
Buat partisi baru dengan kapasistas 20 GB untuk root.

- ![bootable](./assets/18.png)
Pastikan set *bootable flag* ke on pada partisi root supaya bisa digunakan untuk booting.

- ![storage partition](./assets/23.png)
![storage partition](./assets/24.png)
Pada FREE SPACE yang tersisa, buat partisi baru dengan kapasitas 5 GB dan atur *mount option* ke `/storage`.

- ![swap partition](./assets/25.png)
![swap partition](./assets/26.png)
Pada FREE SPACE yang tersisa, buat partisi baru dengan kapasitas 1.3 GB sebagai swap area.

- ![finish partition](./assets/27.png)
Setelah selesai membuat partisi, arahkan pada *finish partitioning* dan continue.
<br>
**4. Package Manager**<br>
- ![region] (./assets/28.png)<br>
Selanjutnya adalah konfig package manager, pilih Indonesia pada *Archive Country*.

- ![archive mirror](./assets/29.png)<br>
Lalu pilih `kebo.pens.ac.id` pada archive mirror yang tersedia, pastikan device tersambung pada internet. Selanjutnya adalah tunggu hingga proses download dan instalasi package selesai.
<br>
**5. GRUB Bootloader**<br>
- ![grub](./assets/30.png)<br>
Langkah selanjutnya adalah menginstall GRUB Bootloader yang berfungsi untuk melakukan proses booting. Arahkan instalasi pada partisi hard disk yang sudah tersedia.
<br>

### Finishing
![grub](./assets/31.png)
![grub](./assets/32.png)
![grub](./assets/33.png)<br>
Jika proses setup sudah selesai maka Debian sudah berhasil terinstall dan bisa login menggunakan user dan password yang telah dibuat sebelumnya.
<br>
> Terima Kasih.
