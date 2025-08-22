# LAB-41-Switch
Jum'at 22 Agustus 2025  
  
# VLAN
  VLAN merupakan sebuah metode yang sering digunakan untuk mendistribusikan beberapa segmen jaringan berbeda pada perangkat router dengan interface ethernet fisik yang terbatas. Dengan VLAN ini kita bisa membuat sebanyak **4095** segmen LAM dalam sebuah interface. Dalam pembuatan VLAN terdapat sebuah paramater utama yaitu Core Port (tagged) dan Edge Port (Untagged). Mungkin pada istilah lain kedua paramater tersebut lebih dikenal sebagai Trunk Port dan Access port.  
  VLAN menjadi sangat penting juga VLAN ini digunakan, yaitu ketika network dapat menjadi semakin besar skalanya dan traffic broadcast menjadi beban seluruh network. 

# Konfigurasi VLAN 
  1. Pastikan R Utama sudah memiliki konfigurasi dasar sampai terhubung ke internet.
![](IMAGES/)  
![](IMAGES/)  
  2. Kemudian selanjutnya adalah router utama ini akan saya gunakan untuk distribusi kebawah mengunakan 2 VLAN, caranya buat interface baru, di **interface > add > VLAN**. Tambahkan 2 buah VLAN dengan ID 10 dan 200.  
![](IMAGES/)
  3. Tambahkan IP untuk router karna nanti akan digunakan sebagai gateway. **IP > Address**. Agar interface vlan100 ini akan memberikan IP 172.31.1.x dan vlan200 akan memberikan 192.168.30.x.  
![](IMAGES/)  
![](IMAGES/)  
![](IMAGES/)  
  4. Agar lebih mudah, disini kita akan membuat DHCP server untuk masing-masing VLAN interface.

# Konfigurasi VLAN pada perangkat Routerboard yang memiliki Switch Chipset

# Pembahasan  
1. VLAN Trunking
     Jika membawa lebih dari 2 informasi VLAn maka disebut VLAN Trunking.  
3. VLAN Access
     Untuk laptop atau client yanf terkoneksi dari ether2 atau ether3 dinamakan dengan VLAN Access.  
