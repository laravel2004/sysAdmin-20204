```
{
    Nama    : Agung Dwi Nugroho
    NRP     : 3122600006
    Kelas   : 2 STr IT A
}
```

# Perbedaan Command `$ sudo` dan `$ visudo`

### Command `$ sudo`:
Command `$ sudo` atau *superuser do* berfungsi untuk memberikan kemampuan kepada user tertentu untuk menjalankan beberapa atau semua command sebagai root sambil melakukan logging command dan argumen. `$ sudo` berjalan pada basis per-command dan bukan merupakan pengganti untuk shell.<br>
Beberapa fitur yang terdapat pada `$ sudo` adalah:
- Kemampuan untuk membatasi command apa yang dapat dijalankan user pada basis per-host.
- Loggin pada setiap command (memberikan audit yang jelas akan siapa yang menjalankan suatu command)
- Timeout `$ sudo` yang dapat dikonfigurasi.
- Kemampuan untuk menggunakan file konfgurasi yang sama pada machine berbeda.

### Command `$ visudo`:
Command `$ visudo` merupakan *command line utility* yang berfungsi untuk mengedit file pada direktori `/etc/sudoers` secara aman. Selain itu juga akan membuka direktori `/etc/sudoers` menggunakan antarmuka editor vim secara default, meskipun hal ini dapat diedit menggunakan editor lain pada environment variabel. <br>
Hal ini juga mencegah pengeditan berulang yang terjadi pada locks, dan menjalankan *sanity check* serta melakukan cek pada *parse error*.

> Terima Kasih.