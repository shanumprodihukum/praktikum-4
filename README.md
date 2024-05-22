)# praktikum-4
CREATE TABLE pegawai (
  idpegawai VARCHAR(10),
  nama_depan VARCHAR(50),
  nama_belakang VARCHAR(50),
  email VARCHAR(100),
  telepon VARCHAR(15),
  tgl_kontrak DATE,
  id_job VARCHAR(10),
  gaji INT,
  tunjangan INT
);
![ss1](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/864a350e-10eb-46c0-8c05-24ebbaaca0b2)
![ss2](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/06a70037-55ba-4bde-b3cb-727c8305fa42)
INSERT INTO pegawai (idpegawai, nama_depan, nama_belakang, email, telepon, tgl_kontrak, id_job, gaji, tunjangan) VALUES
("E001", "Gojo", "Satoru", "gjsatoru@gmail.com", "08123456719", "2006-01-18", "10001", 2000000, 500000),
("E002", "Raja", "Iblis", "sukuna@gmail.com", "08123456710", "2005-03-28", "10002", 2000000, 200000),
("E003", "Itadori", "Yuji", "itadori@yahoo.com", "68123456711", "2004-06-17", "L0003", 1500008, NULL),
("E004", "Mugiwara", "Luffy", "mugiwara@yahoo.com", "08123456712", "2004-03-19", "10004", 1500000, 9),
("E005", "Rin", "Okumura", "okumura@gmail.com", "08123456713", "2006-03-18", "L0005", 1250000, 9),
("E006", "Megumi", "Fushiguro", "megumi@yahoo.com", "08123456714", "2002-09-17", "L0006", 1750000, NULL);
![image](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/a455c656-b3a1-447c-a35d-9d34a83d5bd
1.Untuk menampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000, Anda dapat menggunakan perintah SQL SELECT dengan klausa WHERE dan operator NOT IN. Berikut adalah contoh kode SQL untuk melakukan hal tersebut:
SELECT *
FROM pegawai
WHERE gaji NOT IN (2000000, 1250000);
![ss3](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/abc605ad-49f1-43d9-a8d2-b02e0b1b9851)

2.Untuk menampilkan pegawai yang tunjangannya NULL, Anda dapat menggunakan perintah SQL SELECT dengan klausa WHERE dan operator IS NULL. Berikut adalah contoh kode SQL untuk melakukan hal tersebut:
SELECT *
FROM pegawai
WHERE tunjangan IS NULL;
![ss4](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/270e553a-c7a5-4b80-b99a-73e0b2f98d65)

 3.Untuk menampilkan pegawai yang tunjangannya tidak NULL, Anda dapat menggunakan perintah SQL SELECT dengan klausa WHERE dan operator IS NOT NULL. Berikut adalah contoh kode SQL untuk melakukan hal tersebut:

SELECT *
FROM pegawai
WHERE tunjangan IS NOT NULL;
![ss5](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/97db4b09-6e41-4b6b-9f79-636c8a244f27)
4.Untuk menampilkan atau menghitung jumlah baris atau record dalam tabel pegawai, Anda dapat menggunakan perintah SQL SELECT dengan fungsi COUNT. Berikut adalah contoh kode SQL untuk melakukannya:
![ss6](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/d61964a7-c31d-479b-92ea-3e09120a915e)
SELECT COUNT(*) AS jumlah_pegawai
FROM pegawai;

    5. Untuk menghitung jumlah total gaji di tabel pegawai, Anda dapat menggunakan perintah SQL SELECT dengan fungsi agregat SUM. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT SUM(gaji) AS total_gaji
FROM pegawai;
![ss7](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/b147c874-bb0e-4ff3-bd9a-e27617961e30)

    6.Untuk menghitung rata-rata gaji pegawai, Anda dapat menggunakan perintah SQL SELECT dengan fungsi agregat AVG. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT AVG(gaji) AS rata_gaji
FROM pegawai;
![ss8](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/3393f3db-c9ef-4d34-9d9c-b995fc6fa304)

 7.Untuk menampilkan gaji terkecil dari tabel pegawai, Anda dapat menggunakan perintah SQL SELECT dengan fungsi agregat MIN. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT MIN(gaji) AS gaji_terkecil
FROM pegawai;
![ss9](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/3f2b1b8d-1fe0-4cb9-acac-abe37bf349b8)

8.Untuk menampilkan gaji terbesar dari tabel pegawai, Anda dapat menggunakan perintah SQL SELECT dengan fungsi agregat MAX. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT MAX(gaji) AS gaji_terbesar
FROM pegawai;
![ss10](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/66853df5-1bee-4f18-a556-4437b5d2538f)



