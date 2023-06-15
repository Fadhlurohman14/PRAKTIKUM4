# Praktikum4

```
Nama    : FADHLUROHMAN FATIKH NAVINTINO
NIM     : 312210368
Kelas   : TI.22.A4
```

# Query Filtering

Query filtering merujuk pada proses menyaring atau membatasi hasil query berdasarkan kriteria tertentu.Query filtering memungkinkan kita untuk menentukan kriteria atau kondisi tertentu yang harus dipenuhi oleh data yang akan ditampilkan.Dalam konteks pemrograman dan pengembangan aplikasi, query filtering biasanya dilakukan dengan menggunakan pernyataan atau sintaks yang mendefinisikan kriteria untuk memfilter data. Ini dapat melibatkan penggunaan operator logika seperti "AND" dan "OR", operator perbandingan seperti ">", "<", atau "EQUALS", serta penggunaan klausa seperti "WHERE" dalam SQL untuk membatasi hasil query.

# Tugas Praktikum

- Buat Table pegawai dan isi datanya seperti berikut

  ![img](SS/1.png)

1. Tampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000 !

- Input

```sql
SELECT * FROM pegawai WHERE gaji <> 2000000 AND gaji <>125000;
```

- Output

  ![img](SS/2.png)

2. Tampilkan pegawai yang tunjangannya NULL!

- Input

```sql
SELECT * FROM pegawai WHERE tunjangan IS NULL;
```

- Output

  ![img](SS/3.png)

3. Tampilkan pegawai yang tunjangannya tidak NULL!

- Input

```sql
SELECT * FROM pegawai WHERE tunjangan IS NOT NULL;
```

- Output

  ![img](SS/4.png)

4. Tampilkan/hitung jumlah baris/record tabel pegawai!

- Input

```sql
SELECT COUNT(*) AS jumlah_baris FROM pegawai;
```

- Output

  ![img](SS/5.png)

5. Tampilkan/hitung jumlah total gaji di tabel pegawai!

- Input

```sql
SELECT SUM(gaji) AS total_gaji FROM pegawai;
```

- Output

  ![img](SS/6)

6. Tampilkan/hitung rata-rata gaji pegawai!

- Input

```sql
SELECT AVG(gaji) AS rata_gaji FROM pegawai;
```

- Output

  ![img](SS/7.png)

7. Tampilkan gaji terkecil!

- Input

```sql
SELECT MIN(gaji) AS gaji_terkecil FROM pegawai;
```

- Output

  ![img](SS/8.png)

8. Tampilkan gaji terbesar!

- Input

```sql
SELECT MAX(gaji) AS gaji_terbesar FROM pegawai;
```

- Output

  ![img](SS/9.png)

  # Tugas Praktikum

- Buat table hewan dan isi datanya seperti berikut:

  ![img](SS/10.png)

1. Tampilkan jumlah hewan yang dimiliki setiap owner.

- Input

```sql
SELECT owner, COUNT(*) AS jumlah_hewan FROM hewan GROUP BY owner;
```

- Output

  ![img](SS/11.png)

2. Tampilkan jumlah hewan berdasarkan spesies

- Input

```sql
SELECT species, COUNT(*) AS jumlah_hewan FROM hewan GROUP BY species;
```

- Output

  ![img](SS/12.png)

3. Tampilkan jumlah hewan berdasarkan jenis kelamin

- Input

```sql
SELECT sex, COUNT(*) AS jumlah_hewan FROM hewan GROUP BY sex;
```

- Output

  !![img](SS/13.png)

4. Tampilkan jumlah hewan berdasarkan spesies dan jenis kelamin

- Input

```sql
SELECT sex, COUNT(*) AS jumlah_hewan FROM hewan GROUP BY sex;
```

- Output

  ![img](SS/14.png)

5. Tampilkan jumlah hewan berdasarkan spesis (cat dan dog saja)
   dan jenis kelamin
   - Input
   ```sql
   SELECT species,sex, COUNT(*) AS jumlah_hewan FROM hewan
   WHERE species IN('Cat','Dog')
   GROUP BY species,sex;
   ```

- Output

  ![img](SS/15.png)

6. Tampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui
   saja

   - Input

   ```sql
   SELECT sex, COUNT(*) AS jumlah_hewan FROM hewan
   WHERE sex IN('f','m')
   GROUP BY sex;
   ```

   - Output
   
     ![img](SS/16.png)

# Evaluasi dan Pertanyaan

• Tulis semua perintah-perintah SQL percobaan di atas beserta
outputnya!
• Beri kesimpulan Anda!

- Kesimpulan dari query filtering adalah sebagai berikut:

  1. Query filtering adalah proses menyaring atau membatasi hasil query berdasarkan kriteria tertentu.
  2. Query filtering digunakan untuk mendapatkan data yang spesifik dan relevan dengan kebutuhan kita.
  3. Query filtering melibatkan penggunaan operator logika, operator perbandingan, dan klausa seperti "WHERE" dalam SQL.
  4. Query filtering memungkinkan kita untuk menentukan kondisi atau kriteria tertentu yang harus dipenuhi oleh data yang akan ditampilkan.
  5. Contoh penggunaan query filtering meliputi memfilter data berdasarkan nilai tertentu, memfilter data berdasarkan kategori, dan memfilter data berdasarkan hubungan dengan data lainnya.