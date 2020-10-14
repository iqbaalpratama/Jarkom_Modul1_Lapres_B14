# **Praktikum_Jarkom_Modul1_B14**
## **A. Display Filter**
### 8. Cari objek apa saja yang didownload (RETR) dari koneksi FTP dengan Microsoft FTP Service!
- Langkah pertama adalah mencari ip address dari Microsoft FTP Service dengan filter `ftp contains "Microsoft FTP Service"`.
![alt text](https://github.com/iqbaalpratama/Praktikum_Jarkom_B14/blob/main/data/jawaban8a.PNG?raw=true)
- Berikutnya, kita cari dari FTP yang memiliki info RETR yang berasal dari ip tersebut dengan filter `ip.src == 192.168.0.128 && ftp contains "RETR"`.
![alt text](https://github.com/iqbaalpratama/Praktikum_Jarkom_B14/blob/main/data/jawaban8b.PNG?raw=true)
- Sehingga kita ketahui bahwa objek yang didownload dari koneksi dengan Microsoft FTP Service adalah `Readme` dan `license.txt`.
### 9. Cari username dan password ketika login FTP pada localhost!
- Ip server ketika login FTP pada localhost adalah `127.0.0.1`. Kemudian kita filter packet yang mengandung `USER` dan `PASS` dengan filter `ip.scr_host == 127.0.0.1 && (ftp contains "USER" || ftp contains "PASS")`.
![alt text](https://github.com/iqbaalpratama/Praktikum_Jarkom_B14/blob/main/data/jawaban9.PNG?raw=true)

## **B. Capture Filter**
### 11. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
### 12. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!
### 13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
### 14. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
### 15. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!
