# portswigger-lab-retrieve-data-from-other-tables

## resource belajar
https://portswigger.net/web-security/sql-injection/union-attacks/lab-retrieve-data-from-other-tables

## step by step
1. Lab ini memiliki kerentanan pada filter category yang dapat membaca data dari tabel lain.
2. Kita bisa lakukan injection sql langsung pada query filter dengan payload sebagai berikut untuk mencari kredensial.
<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/79e54bcb-b1b6-41a7-a675-f946fd237b9a" />

3. coba login dengan kredensial admin.
<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/c0794861-06af-4644-a9d9-8bafdb162cb6" />

4. Challenge berhasil diselesaikan
   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/7a7ad3e7-378b-48af-a1c3-4e9e527bbe2d" />

