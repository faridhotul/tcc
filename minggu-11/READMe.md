# PRAKTIKUM TEKNOLOGI CLOUD - PERTEMUAN 11

## NAMA : ARVIAN EKA SAPUTRA (175410041) || FARIDHOTUL KHASANAH (175410026) || ROCHMAD WIDIANTO (185410014)
## PRAKTIKUM - IAAS
---------------------------------------------
**1. KONSEP IAAS**

**IaaS (Infrastruktur as a Service)** jika diartikan menurut bahasa Indonesia adalah layanan infrastruktur komputasi awan. Layanan cloud IaaS biasanya terdiri dari satu paket perangkat hardware komputer berupa virtualisasi, dengan jaringan internet, dukungan alamat IP, bandwitch, keseimbangan beban, jaminan online secara realtime (koneksi ke internet secara kontinyu) serta keamanan pada ruang lingkup satu unit layanan IaaS. Provider umumnya menyediakan layanan dengan berbagai spesifikasi, yakni CPU, RAM serta Data Storage dalam bentuk virtualisasi.

![gambar Konsep](konsep-Cloud-IaaS.jpg)

**2. BERBAGAI SOFTWARE IAAS**

2.1 . AT & T Cloud Solutions
Dengan persembahan jaringan global AT & T, Anda dapat mengoptimalkan komputasi,penyimpanan, perangkat lunak, pengembangan dan bahkan sumber daya jaringan dalam lingkungan berbasis cloud. AT & T menawarkan end-to-end kapasitas pengiriman pada skala global, didukung oleh puluhan tahun pengalaman dan keahlian terbesar. Bersama dengan ekosistem penyedia layanan kami yang luas, kami menyediakan luasnya besar kemampuan cloud, keamanan, dan jaringan. Semua melalui titik kontak.

![gambar contoh](AT&TCloudSolution.png)

2.2 Amazon EC2
Amazon EC2 dalah platform komputasi berupa virtual computer yang dapat di kustomisasi maupun di kembangkan dengan menggunakan prinsip cluster dan load balance. Untuk deployment nya sendiri sangat mudah sekali karena hanya perlu memilih image yang disebut AMI (Amazon Machine Instances) dan setup hanya perlu 5-10 menit.

![gambar contoh](amazon.png)

2.3  NaviSite
NaviSite, Inc., merupakan Time Warner Cable Company, adalah penyedia internasional terkemuka dari pelayanan dan pengaturan aplikasi-aplikasi kelas enterprise dan hosting cloud. NaviSite menyediakan rangkaian lengkap dari layanan yang dikelola serta dapat diandalkan dan terukur, termasuk pelayanan aplikasi, Hosting perusahaan yang terdepan dalam industri, dan pelayanan pengaturan Cloud untuk organisasi ingin melakukan outsourcing infrastruktur TI dan membantu menurunkan modal serta biaya operasional. Konsumen perusahaan bergantung pada NaviSite untuk solusi khusus, yang disampaikan melalui pusat data kelas internasional yang canggih.

![gambar contoh](navisite.png)

**3. GETTING STARTED IAAS**
Instalasi Proxmox

![gambar 1](1.png)

![gambar 2](2.png)

![gambar 3](3.png)

![gambar 4](4.png)

![gambar 5](5.png)

![gambar 6](6.png)

![gambar 7](7.png)

![gambar 8](8.png)

![gambar 9](9.png)

![gambar 10](10.png)

![gambar 11](11.png)

![gambar 12](12.png)

![gambar 13](13.png)

![gambar 14](14.png)

![gambar 15](15.png)

![gambar 16](16.png)

![gambar 17](17.png)

![gambar 18](18.png)

![gambar 19](19.png)

![gambar 20](20.png)

![gambar 21](21.png)

![gambar 22](22.png)

![gambar 23](23.png)

![gambar 24](24.png)

![gambar 25](25.png)

![gambar 26](26.png)

![gambar 27](27.png)

![gambar 28](28.png)

![gambar 29](29.png)

![gambar 30](30.png)



**4. ARSITEKTUR DAN KONSEP DEPLOYMENT PADA PROXMOX**

 ![gambar contoh](arsitektur-proxmox.jpg)

 Proxmox mendukung beberapa metode manajemen user, di antaranya adalah LDAP, Active Diretory (AD), Linux PAM, dan Proxmox VE authentication server. LDAP dan AD membutuhkan server eksternal khusus untuk autentikasi. Sedangkan Linux PAM dan Proxmox VE authentication merupakan autentikasi internal. Konsep manajemen user ini memungkinkan kita untuk membuat user dan group lalu memberikan role dan permission untuk pengelolaan Proxmox VE. Kita juga dapat memberikan akses mengubah konfigurasi komponen seperti storage, VM, atau sistem ke user/group tertentu saja. Kita bahkan dapat membuat user/group yang hanya dapat melihat tapi tidak dapat mengubah konfigurasi.