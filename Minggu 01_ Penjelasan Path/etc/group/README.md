```
{
    Nama    : Agung Dwi Nugroho
    NRP     : 3122600006
    Kelas   : 2 STr IT A
}
```
# Direktori /etc/group

Disini saya ingin menjelaskan tingkatan user yang ada di debian menurut folder `/etc/group`
directory ini digunakan untuk mengatur tingkatan user yang ada di OS debian
<br />

Setingan atau cara membaca group user dengan adalah seperti ini :
<br />
`nama_grup:password:ID_grup:anggota1,anggota2,...`
<br />
Sebagai contoh :
<br />
`users:x:1000:john,mary,bob`
<br />
<br />

**Penjelasan untuk membaca**

1. Nama grup adalah "users".<br />
2. Password mungkin terdapat karakter 'x' atau kosong (tergantung pada konfigurasi sistem).<br />
3. ID grup adalah 1000.<br />
4. Anggota grup adalah john, mary, dan bob.<br />
