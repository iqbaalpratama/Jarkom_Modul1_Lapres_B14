# **Jarkom_Modul1_Lapres_B14**
## **A. Display Filter**
### 1. Sebutkan webserver yang digunakan pada "testing.mekanis.me"!

### 2. Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!

### 3. Cari username dan password ketika login di "ppid.dpr.go.id"!

### 4. Temukan paket dari web-web yang menggunakan basic authentication method!

### 5. Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!

### 6. Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).

### 7. Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut! Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf".


### 8. Cari objek apa saja yang didownload (RETR) dari koneksi FTP dengan Microsoft FTP Service!
- Langkah pertama adalah mencari ip address dari Microsoft FTP Service dengan filter `ftp contains "Microsoft FTP Service"`.
![alt text](https://github.com/iqbaalpratama/Praktikum_Jarkom_B14/blob/main/data/jawaban8a.PNG?raw=true)
- Berikutnya, kita cari dari FTP yang memiliki info RETR yang berasal dari ip tersebut dengan filter `ip.src == 192.168.0.128 && ftp contains "RETR"`.
![alt text](https://github.com/iqbaalpratama/Praktikum_Jarkom_B14/blob/main/data/jawaban8b.PNG?raw=true)
- Sehingga kita ketahui bahwa objek yang didownload dari koneksi dengan Microsoft FTP Service adalah `Readme` dan `license.txt`.

### 9. Cari username dan password ketika login FTP pada localhost!
- Ip server ketika login FTP pada localhost adalah `127.0.0.1`. Kemudian kita filter packet yang mengandung `USER` dan `PASS` dengan filter `ip.scr_host == 127.0.0.1 && (ftp contains "USER" || ftp contains "PASS")`.
![alt text](https://github.com/iqbaalpratama/Praktikum_Jarkom_B14/blob/main/data/jawaban9.PNG?raw=true)

### 10. Cari file .pdf di wireshark lalu download dan buka file tersebut! clue: "25 50 44 46" 
- Berdasarkan klu yang diberikan, kode tersebut dicari dengan `Ctrl + f` dan tipe data Hex value.

## **B. Capture Filter**
### 11. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
- Pada bagian capture filter masukan `port 21` untuk  mengambil paket yang mengandung port 21.

### 12. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!
- Pada bagian capture filter masukan `src port 80` untuk  mengambil paket yang berasal dari port 80.

### 13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
- Pada bagian capture filter masukan `dst port 443` untuk  mengambil paket yang menuju port 443.

### 14. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
- Pada bagian capture filter masukan `dst port 443` untuk  mengambil paket yang menuju port 443.

### 15. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!
- Pada bagian capture filter masukan `dst host monta.if.its.ac.id` untuk  mengambil paket yang tujuannya ke monta.if.its.ac.id.
