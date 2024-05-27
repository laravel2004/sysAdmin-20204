```json
{
    Nama    : "Agung Dwi Nugroho"
    NRP     : 3122600006
    Kelas   : "2 STr IT A"
}
```

# Proses Iteratif DNS Server
Ketika seorang pengguna mengetikkan URL di browser, terjadi serangkaian proses yang kompleks untuk menghubungkan pengguna ke situs web yang dimaksud. Berikut adalah rangkuman dari proses tersebut: <br>

1. **DNS Request ke Local DNS:** Pertama, browser melakukan permintaan DNS (Domain Name System) ke server DNS lokal untuk mencari alamat IP dari situs web yang diminta, contohnya www.example.com

2. **DNS Request Diteruskan ke Forwarder:** Jika server DNS lokal tidak memiliki informasi tentang alamat IP tersebut, permintaan DNS diteruskan ke server DNS eksternal yang disebut forwarder, misalnya 202.9.85.3.

3. **DNS Server Meneruskan Request ke Root Server:** Jika forwarder tidak memiliki informasi tersebut, permintaan DNS diteruskan ke root server, yang merupakan tahap awal dari proses pencarian DNS.

4. **Root Server Membalas ke DNS Server/Forwarder:** Root server membalas dengan mengarahkan DNS server atau forwarder ke server terdekat yang mengelola domain top-level, seperti ".com" dalam kasus ini. Ini dilakukan berdasarkan anycast terdekat.

5. **DNS Server Menanyakan ke .com Mengenai IP:** DNS server kemudian mengirim permintaan ke server yang mengelola domain top-level ".com" untuk mendapatkan alamat IP dari www.example.com.

6. **.com Membalas dengan IP Network:** Server ".com" membalas dengan memberikan informasi tentang alamat IP yang terkait dengan www.example.com.

7. **DNS Server Mengirim Permintaan ke NS.example.com:** DNS server kemudian mengirimkan permintaan ke server nama (NS) yang ditunjuk oleh ".com" untuk mendapatkan alamat IP www.example.com.

8. **NS.example.com Membalas dengan Alamat IP:** Server NS.example.com membalas dengan memberikan alamat IP www.example.com kepada DNS server.

9. **DNS Server Mengembalikan ke Client:** DNS server akhirnya mengembalikan alamat IP www.example.com ke browser pengguna sebagai respons atas permintaan DNS awal.

<br>

Dalam proses ini, penting untuk dicatat bahwa alamat IP yang diperoleh dari server DNS akan disimpan di cache sesuai dengan TTL (Time to Live), sehingga proses iteratif hanya berlangsung sekali untuk permintaan yang sama selama waktu TTL yang ditentukan. Hal ini membantu dalam meningkatkan efisiensi dan kinerja sistem DNS secara keseluruhan.

> Terima Kasih