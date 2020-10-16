# **Jarkom_Modul1_Lapres_B14**
## **A. Display Filter**
### 1. Sebutkan webserver yang digunakan pada "testing.mekanis.me"!
- Langkah pertama yaitu melakukan dispalay filter dengan command `http contains "testing.mekanis.me"`.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban1a.png?raw=true)
- Berikutnya pilih salah satu paket dan kemudian lihat detail paket tersebut untuk mengetahui webserver yang digunakan dengan follow TCP Stream
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban1b.png?raw=true)
- Lihat webserver yang digunakan pada bagian Server berikut
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban1c.png?raw=true)
### 2. Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!
- Cara menyimpan gambar tersebut yaitu Export HTTP Object seperti berikut
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban2a.png?raw=true)
- Kemudian lakukan text filter dengan `Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg` dan save hasil yang muncul
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban2b.png?raw=true)
- Berikut ini hasil gambar yang di-download
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban2c.png?raw=true)
### 3. Cari username dan password ketika login di "ppid.dpr.go.id"!
- Caranya yaitu dengan menggunakan display filter `http contains "ppid.dpr.go.id" && http.request.method == "POST"`
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban3a.png?raw=true)
- Kemudian scroll ke bawah hingga menemukan HTML Form URL Encoded sehingga terlihat username dan password ketika login di `ppid.dpr.go.id` seperti berikut
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban3b.png?raw=true)
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban3c.png?raw=true)
### 4. Temukan paket dari web-web yang menggunakan basic authentication method!
- Cara yang digunakan yaitu dengan display filter `http.authbasic` sehingga daftar paket yang menggunakan basic authentification seperti berikut
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban4a.png?raw=true)
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban4b.png?raw=true)
### 5. Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!
- Cara yang digunakan yaitu dengan display filter `http contains "aku.pengen.pw" && http.authbasic` dan pilih salah satu paket
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban5a.png?raw=true)
- Kemudian pada bagian Authorization nantinya akan ada Credentials yang merupakan username dan password dimana usernamenya `kakakgamtenk` dan passwordnya `hartatahtabermuda`
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban5b.png?raw=true)
- Setelah itu login di `aku.pengen.pw` dengan username dan password yang sudah ditemukan sebelumnya dan menjawab pertanyaan pada web tersebut
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban5c.png?raw=true)

### 6. Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).
- Langkah pertama yaitu dengan display filter `ftp-data.command contains "Answer.zip"` untuk mencari file `Answer.zip`
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban6a.png?raw=true)
- Kemudian gunakan follow TCP Stream untuk melihat detail paket, kemudian pilih tipe data Raw untuk nantinya digunakan melihat data
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban6b.png?raw=true)
- Save as data tersebut dengan ekstensi `.zip`
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban6c.png?raw=true)
- Mencari file `zipkey.txt` untuk mengetahui password dari file `Answer.zip` dengan display filter `ftp-data.command contains "zipkey.txt"`
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban6d.png?raw=true)
- Kemudian gunakan follow TCP Stream untuk melihat detail paket serta set tipe data ASCII untuk bisa membaca data file tersebut. Data yang dihasilkan tersebut merupakan password dari file `Answer.zip`
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban6e.png?raw=true)
- Masukkan password tersebut untuk membuka file `Answer.zip` dan nantinya akan ada file `Open This.pdf` yang dicari
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban6f.png?raw=true)
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban6g.png?raw=true)
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban6h.png?raw=true)

### 7. Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut! Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf".
- Langkah pertama yaitu dengan display filter `ftp-data contains "Yes.pdf"` untuk mencari file zip yang memiliki file `Yes.pdf` di dalamnya
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban7a.png?raw=true)
- Kemudian gunakan follow TCP Stream untuk melihat detail paket, kemudian pilih tipe data Raw untuk nantinya digunakan melihat data
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban7b.png?raw=true)
- Save as data tersebut dengan ekstensi `.zip`
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban7c.png?raw=true)
- Buka file hasil save data tersebut kemudian nanti akan ada file `Yes.pdf` yang dicari
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban7d.png?raw=true)
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban7e.png?raw=true)
### 8. Cari objek apa saja yang didownload (RETR) dari koneksi FTP dengan Microsoft FTP Service!
- Langkah pertama adalah mencari ip address dari Microsoft FTP Service dengan filter `ftp contains "Microsoft FTP Service"`.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban8a.PNG?raw=true)
- Berikutnya, kita cari dari FTP yang memiliki info RETR yang berasal dari ip tersebut dengan filter `ip.src == 192.168.0.128 && ftp contains "RETR"`.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban8b.PNG?raw=true)
- Sehingga kita ketahui bahwa objek yang didownload dari koneksi dengan Microsoft FTP Service adalah `Readme` dan `license.txt`.

### 9. Cari username dan password ketika login FTP pada localhost!
- Ip server ketika login FTP pada localhost adalah `127.0.0.1`. Kemudian kita filter packet yang mengandung `USER` dan `PASS` dengan filter `ip.scr_host == 127.0.0.1 && (ftp contains "USER" || ftp contains "PASS")`.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban9.PNG?raw=true)

### 10. Cari file .pdf di wireshark lalu download dan buka file tersebut! clue: "25 50 44 46" 
- Berdasarkan clue yang diberikan, kode tersebut dicari dengan `Ctrl + F` dan tipe data Hex value kemudian mengetikkan clue `25 50 44 46`
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban10a.png?raw=true)
- Kemudian dari hasil yang diberikan digunakan follow TCP Stream untuk melihat data, pilih tipe data Raw untuk nantinya digunakan melihat data
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban10b.png?raw=true)
- Save as data tersebut dengan ekstensi `.pdf` dan hasilnya adalah
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban10c.png?raw=true)
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban10d.png?raw=true)
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban10e.png?raw=true)

## **B. Capture Filter**
### 11. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
- Pada bagian capture filter masukan `port 21` untuk  mengambil paket yang mengandung port 21.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban11a.PNG?raw=true)
- Hasilnya maka seperti gambar di bawah ini. Namun karena port 21 tidak digunakan maka hasilnya kosong.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban11b.PNG?raw=true)

### 12. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!
- Pada bagian capture filter masukan `src port 80` untuk  mengambil paket yang berasal dari port 80.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban12a.PNG?raw=true)
- Hasilnya maka seperti gambar di bawah ini.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban12b.PNG?raw=true)

### 13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
- Pada bagian capture filter masukan `dst port 443` dan pilih wifi atau ethernet untuk  mengambil paket yang menuju port 443.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban13a.PNG?raw=true)
- Hasilnya maka seperti gambar di bawah ini.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban13b.PNG?raw=true)
### 14. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
- Untuk mendapatkan ip komputer sendiri kita bisa mencarinya pada cmd dengan memasukkan command `ipconfig`. Pada bagian wifi tertera ipv4 yang menunjukan ip ketika terhubung ke wifi. 
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban14a.PNG?raw=true)
- Pada bagian capture filter masukan `src host 192.168.43.93` dan pilih wifi untuk mengambil paket yang berasal dari ip sendiri.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban14b.PNG?raw=true)
- Hasilnya maka seperti gambar di bawah ini.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban14c.PNG?raw=true)

### 15. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!
- Pada bagian capture filter masukan `dst host monta.if.its.ac.id` dan pilih wifi atau ethernet untuk  mengambil paket yang tujuannya ke monta.if.its.ac.id.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban15a.PNG?raw=true)
- Hasilnya maka seperti gambar di bawah ini.
![alt text](https://github.com/iqbaalpratama/Jarkom_Modul1_Lapres_B14/blob/main/data/jawaban15b.PNG?raw=true)
