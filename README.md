# **Praktikum_Jarkom_Modul1_B14**
## **A. Display Filter**
### 8. Cari objek apa saja yang didownload (RETR) dari koneksi FTP dengan Microsoft FTP Service!
- Langkah pertama adalah mencari ip address dari Microsoft FTP Service dengan filter `ftp contains "Microsoft FTP Service"`.
![alt text](https://github.com/iqbaalpratama/Praktikum_Jarkom_B14/blob/main/data/jawaban8a.PNG?raw=true)
- Berikutnya, kita cari dari FTP yang memiliki info RETR yang berasal dari ip tersebut `ip.src == 192.168.0.128 && ftp contains "RETR"`.
![alt text](https://github.com/iqbaalpratama/Praktikum_Jarkom_B14/blob/main/data/jawaban8b.PNG?raw=true)

## **B. Capture Filter**
### 11. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
### 12. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!
### 13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
### 14. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
### 15. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!
