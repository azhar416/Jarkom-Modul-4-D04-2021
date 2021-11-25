# Jarkom-Modul-4-D04-2021

1. Daffa Muhamad Azhar [05111940000037]
2. Taqarra Rayhan I [05111940000121]
3. Iwan Dwi Prakoso [05111940000229]

# MODUL 4

![topology](https://github.com/azhar416/Jarkom-Modul-4-D04-2021/blob/main/img/topology.PNG)

## Routing dan Subnetting dengan CISCO

### CIDR

1. Membuat Topology-nya terlebih dahulu pada CISCO

2. Memilih Subnet yang paling optimal

![subnet](https://github.com/azhar416/Jarkom-Modul-4-D04-2021/blob/main/img/CIDR/subnet.PNG)

3. Hitung panjang setiap Subnet

![subnet-length](https://github.com/azhar416/Jarkom-Modul-4-D04-2021/blob/main/img/CIDR/subnet-length.PNG)

4. menggabungkan subnet paling bawah di dalam topologi. Paling bawah berarti subnet yang paling jauh dari internet (gambar awan). Gabungkan hingga tersisa 1 buah Subnet.

![subnet-gabung](https://github.com/azhar416/Jarkom-Modul-4-D04-2021/blob/main/img/CIDR/subnet-gabung.PNG)

5. Menghitung Pembagian IP dengan Pohon.

![pohon](https://github.com/azhar416/Jarkom-Modul-4-D04-2021/blob/main/img/CIDR/pohon.PNG)

6. Membuat tabel pembagian IP

![tabel](https://github.com/azhar416/Jarkom-Modul-4-D04-2021/blob/main/img/CIDR/tabel.PNG)

### Configure

1. Konfigurasi Router

setiap router di config sesuai arah kabel terhadap subnet.

sebagai contoh pada router Foosha akan di konfig terhadap **A5** (mengarah ke router Water7). maka router Foosha akan mengambil salah satu IP dari **A5** dan menggunakan subnet mask **A5** pada kabel yang mengarah ke Water7.

![config-foosha-water7](https://github.com/azhar416/Jarkom-Modul-4-D04-2021/blob/main/img/CIDR/config-foosha-water7.PNG)

Sementara untuk router Water7 akan mengambil IP pada **A5** yang belum diambil oleh Foosha pada kabel yang mengarah ke Foosha.

![config-water7-foosha](https://github.com/azhar416/Jarkom-Modul-4-D04-2021/blob/main/img/CIDR/config-water7-foosha.PNG)

Lakukan hingga semua Subnet Terpenuhi.

2. Konfigurasi Host (PC)

