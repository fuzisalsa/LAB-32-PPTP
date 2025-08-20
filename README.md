# LAB-32-PPTP
tanggal 20 agustus 2025

# konfigurasi PPTP client 
1. masuk ke mikrotik clinet  

![m](p6.PNG)

2. pilih menu  PPP > INTERFACE    
3. klik (+)     
4. pilih tab **dial out** isi parameter:   
   connect to: isikan ip public dari office A   
   masukkan user dan password PPTP sever   
   arahkan profile nya ke **default-encryption**    

![m](p2.PNG)

5. nah secara otomatis kita akan di buatkan interface baru oleh sistem namanya **pptp-out1**.   
dan flag nya R berarti sudah running/terkoneksi.   

![m](p1.PNG)

6. kita bisa lihat di address ip > address    
   klo sudah di tambambahkan nya ip sercara otomatis dari interface **pptp-out1.**   

![m](p4.PNG)

7. jika sudah terkoneksi sekarang kita buat pengaturan routing supaya pengaturan antar LAN yang ada pada office A dan office B bisa saling terkoneksi melalui PPTP tunnel.
   pilih menu ip > routes    
   di bagian dst.address isi dengan ip office A   
   gateway nya interface pptp-out1   

![m](p3.PNG)

9. coba ping ke office A lewat terminal   

![m](p5.PNG)

 
