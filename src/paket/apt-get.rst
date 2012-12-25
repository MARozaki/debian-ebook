apt-get
=======

Tool instalasi ala debian dengan menggunakan ``apt-get`` ini memiliki
kemudahan dibanding dengan cara konvensional ``dpkg`` yang telah dijelaskan
pada subbab sebelumnya. Anda hanya perlu mengetahui nama paketnya saja.
Jika terdapat dependensi (ketergantungan) dengan paket lain, maka
``apt-get`` akan mencari sendiri kemudian menginstal paket tersebut tanpa
harus bersusah payah mencari letak software tersebut.

Format umum pemakaian tool 'apt-get' adalah sebagai berikut::

 debian:~# apt-get [opsi] software1 software2 ...

Instalasi dengan apt-get
------------------------

Untuk instalasi paket software dengan ``apt-get`` dapat menggunakan perintah
berikut::

    debian:~# apt-get install software1 software2 ...

Misal: Penulis ingin menginstal software mozilla, mc, pico, dan parted.
Perintah yang digunakan adalah::

    debian:~# apt-get install mozilla mc pico parted

Menghapus Software
------------------

Untuk menghapus software yang telah terinstal pada Debian GNU/Linux.
Perintah yang digunakan adalah::

    debian:~# apt-get remove software1 software2 ...

Misal: Penulis ingin menghapus software ``pico`` dan ``iceweasel``.
Perintah yang digunakan adalah::

    debian:~# apt-get remove pico iceweasel

Upgrade Distro Debian GNU/Linux
-------------------------------

Untuk meng-upgrade distro Debian GNU/Linux dapat menggunakan perintah
berikut::

    debian:~# apt-get dist-upgrade

Mengunduh Source dari Sebuah Situs
----------------------------------

Untuk mendownload paket software debian GNU/Linux pada sebuah situs dapat
menggunakan perintah berikut::

 debian:~# apt-get –d source software1 software2 ...

.. note::
 Alamat URL tempat source paket software Debian berada harus tercantung pada
 direktori ``/etc/apt/sources.list``

Membersihkan Arsip File Download Software
-----------------------------------------

Untuk membersihkan arsip file download software dapat menggunakan perintah
berikut::

 debian:~# apt-get clean | autoclean

Upgrade Paket Software
----------------------

Untuk meng-upgrade paket software dapat menggunakan perintah berikut::

 debian:~# apt-get upgrade

Update Informasi Daftar Paket Software Baru
-------------------------------------------

Untuk meng-update daftar paket software baru dapat menggunakan perintah
berikut::

debian:~# apt-get update

Dselect
=======

Tool instalasi `dselect` ini memberikan kemudahan kepada user debian
GNU/Linux dalam melakukan instalasi karena dilengkapi dengan tampilan semi
grafis. Anda hanya menyorot opsi [I]nstall jika ingin menginstal atau meng-
upgrade paket software, opsi [R]emove jika ingin menghapus sebuah software
dari sistem, opsi [C]onfig untuk mengkonfigurasi paket software yang belum
terkonfigurasi, dan beberapa opsi lain yang diperlukan. Pengaksesan tool
`dselect` dapat menggunakan perintah berikut::

 debian:~# dselect

Instalasi Software dari CDROM
=============================

Untuk instalasi software dari cdrom pada debian GNU/Linux termasuk untuk
meng-upgrade KDE 3.0 ke KDE 3.1 atau KDE 3.2 dapat dengan mudah
dilakukan. Untuk instalasi software dari cdrom dapat menggunakan perintah
berikut.

apt - Instalasi dengan mode teks
--------------------------------

1. Login ke sistem sebagai user root.
2. Buka command line (konsole) dengan mengklik ikon konsole pada panel.
3. Pada konsole, ketikkan perintah berikut::

 debian:~# apt-cdrom add

4. Masukkan cd installer kemudian ketikkan perintah berikut::

 debian:~# apt-get install namapaket

