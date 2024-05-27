```
{
    Nama    : Agung Dwi Nugroho
    NRP     : 3122600006
    Kelas   : 2 STr IT A
}
```

# Debian
Melansir dari <a>debian.org</a>, Debian merupakan sebuah sistem operasi gratis yang dikembangkan oleh asosiasi bernama **The Debian Project**. Debian merupakan salah satu distribusi Linux dengan ribuan aplikasi untuk memenuhi kebutuhan user. <br>
Hingga sekarang terdapat banyak versi dari Debian. Yang terbaru adalah Debian versi 12 atau dikenal dengan *Bookworm*. Pada repo ini akan meringkas tentang perbedaan Debian versi 11 dengan Debian versi 12 terutama pada sisi kernel, kebutuhan sistem, penerapan systemd, dan package.

### Debian 11 (Bullseye) vs Debian 12 (Bookworm)
<table>
    <tr>
        <th></th>
        <th>Debian 11 Bullseye</th>
        <th>Debian 12 Bookworm</th>
    </tr>
    <tr>
        <th>Versi Kernel</th>
        <td>Linux Kernel Image 5.10</td>
        <td>Linux Kernel Image 6.1</td>
    </tr>
    <tr>
        <th>Kebutuhan Sistem</th>
        <td>
            <ul>
                <li>512MB RAM & 2GB HDD (no desktop)</li>
                <li>2GB RAM & 10GB HDD (with desktop)</li>
            </ul>
        </td>
        <td>
            <ul>
                <li>512MB RAM & 4GB HDD (no desktop)</li>
                <li>2GB RAM & 10GB HDD (with desktop)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <th>Systemd</th>
        <td>Versi 247</td>
        <td>Versi 252</td>
    </tr>
    <tr>
        <th>Package</th>
        <td>
            <ul>
                <li>lilo bootloader digantikan dengan grub2</li>
                <li>mailman 2.1 sudah tidak tersedia</li>
                <li>isdn4linux tidak support dengan kernel</li>
                <li>libappindicator-dev digantikan dengan libayatana-appindicator</li>
                <li>chef sudah tidak tersedia</li>
                <li>Python 2 digantikan dengan Python 3</li>
                <li>wicd connection manager sudah tidak tersedia</li>
            </ul>
        </td>
        <td>
            <ul>
                <li>libnss-ldap digantikan dengan libnss-ldap dan libnss-sss</li>
                <li>fdflush digantikan dengan util-linux</li>
                <li>libgdal-perl sudah tidak tersedia</li>
            </ul>
        </td>
    </tr>
</table>

> Terima Kasih.