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
7.
    Untuk menampilkan gaji terkecil dari tabel pegawai, Anda dapat menggunakan perintah SQL SELECT dengan fungsi agregat MIN. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT MIN(gaji) AS gaji_terkecil
FROM pegawai;
![ss9](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/b77f1d23-f2cc-4a76-8858-6b5e2b6a3371)
8.  Untuk menampilkan gaji terbesar dari tabel pegawai, Anda dapat menggunakan perintah SQL SELECT dengan fungsi agregat MAX. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT MAX(gaji) AS gaji_terbesar
FROM pegawai;
![ss10](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/92ffb409-065d-46fb-bdc6-30e0010f5c80)
 TUGAS PRAKTIKUM 4
 seperti sebelumnya, kita akan membuat tabel terlebih dahulu dengan perintah berikut :

Berikut adalah skrip SQL untuk membuat tabel "hewan" dan mengisinya dengan data yang diberikan:

CREATE TABLE hewan (
  id VARCHAR(2),
  name VARCHAR(10),
  owner VARCHAR(10),
  species VARCHAR(10),
  sex CHAR(1)
);

INSERT INTO hewan (id, name, owner, species, sex)
VALUES
  ('p1', 'Puffball', 'Diane', 'Hamster', 'f'),
  ('p2', 'Claws', 'Gwen', 'Cat', 'm'),
  ('p3', 'Fluffy', 'Haro 1d', 'Cat', 'f'),
  ('p4', 'Buffy', 'Haro 1d', 'Dog', 'f'),
  ('p5', 'Fang', 'Benny', 'Dog', 'm'),
  ('p6', 'Bowser', 'Diane', 'Dog', 'm'),
  ('p7', 'Chirpy', 'Gwen', 'Bird', 'f'),
  ('p8', 'Whistler', 'Gwen', 'Bird', NULL),
  ('p9', 'Slim', 'Benny', 'Snake', 'm');

Perintah di atas akan membuat tabel "hewan" dengan kolom-kolom yang sesuai, yaitu "id", "name", "owner", "species", dan "sex". Kemudian, perintah INSERT INTO digunakan untuk mengisikan data ke dalam tabel tersebut.
![ss11](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/3336dbf2-87ce-4122-b23c-fb7f52c2fea0)
   2. Untuk menampilkan jumlah hewan yang dimiliki setiap owner, Anda dapat menggunakan perintah SQL SELECT dengan klausa GROUP BY dan fungsi agregat COUNT. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT owner, COUNT(*) AS jumlah_hewan
FROM hewan
GROUP BY owner;
![ss12](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/63747076-b614-4c86-8e7f-009ca2bcdb1c)
3.Untuk menampilkan jumlah hewan berdasarkan jenis kelamin, Anda dapat menggunakan perintah SQL SELECT dengan klausa GROUP BY dan fungsi agregat COUNT. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT sex, COUNT(*) AS jumlah_hewan
FROM hewan
<img width="427" alt="ss14" src="https://github.com/shanumprodihukum/praktikum-4/assets/148035386/c3a60c22-6382-4509-ab1d-e641f734afe7">

   4. Untuk menampilkan jumlah hewan berdasarkan spesies dan jenis kelamin, Anda dapat menggunakan perintah SQL SELECT dengan klausa GROUP BY dan fungsi agregat COUNT. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT species, sex, COUNT(*) AS jumlah_hewan
FROM hewan
GROUP BY species, sex;
<img width="437" alt="ss13" src="https://github.com/shanumprodihukum/praktikum-4/assets/148035386/9d215e27-96b3-4030-bc2b-cee19839199f">
5.Untuk menampilkan jumlah hewan berdasarkan spesies (cat dan dog saja) dan jenis kelamin, Anda dapat menggunakan perintah SQL SELECT dengan klausa WHERE untuk memfilter spesies yang diinginkan, serta klausa GROUP BY dan fungsi agregat COUNT. Berikut adalah contoh kode SQL untuk melakukannya:

SELECT species, sex, COUNT(*) AS jumlah_hewan
FROM hewan
WHERE species IN ('Cat', 'Dog')
GROUP BY species, sex;
![ss16](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/672b7993-7606-4c0f-97eb-66361d34397f)
   6. Untuk menampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui saja, Anda dapat menggunakan perintah SQL SELECT dengan klausa WHERE untuk memfilter data berdasarkan jenis kelamin yang tidak NULL, serta klausa GROUP BY dan fungsi agregat COUNT. Berikut adalah contoh kode SQL untuk melakukannya:
      SELECT sex, COUNT(*) AS jumlah_hewan
FROM hewan
WHERE sex IS NOT NULL
GROUP BY sex;
![ss17](https://github.com/shanumprodihukum/praktikum-4/assets/148035386/ac176b74-7453-46d8-a95d-94572be03675)

Evaluasi dan Pertanyaan
    Tulis semua perintah-perintah SQL percobaan di atas beserta outputnya!
terlampir diatas
    Beri kesimpulan Anda!

    Filter Kondisi: Operator relasi (=, >, <, >=, <=, <>) digunakan untuk membandingkan antara dua nilai. Operator BETWEEN digunakan untuk memfilter data dalam rentang tertentu. Operator LIKE atau NOT LIKE digunakan untuk mencari data dengan menggunakan wildcard (_ atau %).

    Operator IN dan IS NULL: Operator IN digunakan untuk memfilter data yang terdapat dalam list tertentu. Operator IS NULL digunakan untuk menampilkan data dengan nilai NULL atau IS NOT NULL untuk menampilkan data yang bukan NULL.

    Pengurutan Data: Perintah ORDER BY digunakan untuk mengurutkan data berdasarkan satu atau beberapa kolom. ASCENDING atau ASC digunakan untuk pengurutan dari nilai terkecil ke terbesar, sedangkan DESCENDING atau DESC digunakan untuk pengurutan dari nilai terbesar ke terkecil.

    Fungsi Agregat: Fungsi agregat (COUNT, SUM, AVG, MIN, MAX) digunakan untuk melakukan perhitungan pada kolom-kolom dalam tabel. COUNT digunakan untuk menghitung jumlah baris, SUM digunakan untuk menjumlahkan nilai kolom, AVG digunakan untuk menghitung rata-rata, MIN digunakan untuk menampilkan nilai terkecil, dan MAX digunakan untuk menampilkan nilai terbesar.

    Klausa GROUP BY: Klausa GROUP BY digunakan untuk mengelompokkan data berdasarkan satu atau beberapa kolom. Ini memungkinkan penggunaan fungsi agregat seperti COUNT, SUM, AVG, MIN, MAX pada setiap grup data.

    Klausa HAVING: Klausa HAVING digunakan untuk memfilter hasil query berdasarkan kondisi tertentu setelah pengelompokan dengan GROUP BY dilakukan. Klausa HAVING berfungsi mirip dengan WHERE, tetapi diterapkan setelah pengelompokan data dilakukan.

Dengan menggunakan kombinasi dari fitur-fitur di atas, kita dapat melakukan filter, pengurutan, dan perhitungan data sesuai dengan kebutuhan kita.
