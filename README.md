![ss1](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/e7c1627a-f67b-4dc9-ad85-4b5c1342b162)# praktikum-4
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
2.Untuk menampilkan pegawai yang tunjangannya NULL, Anda dapat menggunakan perintah SQL SELECT dengan klausa WHERE dan operator IS NULL. Berikut adalah contoh kode SQL untuk melakukan hal tersebut:
SELECT *
FROM pegawai
WHERE tunjangan IS NULL;
 3.Untuk menampilkan pegawai yang tunjangannya tidak NULL, Anda dapat menggunakan perintah SQL SELECT dengan klausa WHERE dan operator IS NOT NULL. Berikut adalah contoh kode SQL untuk melakukan hal tersebut:

SELECT *
FROM pegawai
WHERE tunjangan IS NOT NULL;


