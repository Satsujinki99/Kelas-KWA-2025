# portswigger-lab-retrieve-multiple-values-in-single-column

## resource belajar
https://portswigger.net/web-security/sql-injection/union-attacks/lab-retrieve-multiple-values-in-single-column

## step by step
1. Basis data berisi tabel lain bernama pengguna, dengan kolom bernama nama pengguna dan kata sandi, untuk menyelesaikan lab ini, kita perlu melakukan serangan injeksi SQL UNION yang mengambil semua nama pengguna dan kata sandi, lalu gunakan informasi tersebut untuk masuk sebagai pengguna administrator.
2. Kita bisa gunakan payload `'+UNION+SELECT+NULL,username||'~'||password+FROM+users--` pada query filter yang mempunyai kerentanan untuk mengambil hidden data.
   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/e2ffaecb-1754-4a97-9f19-40d890d812f1" />
3. Coba login dengan kredensial administrator
<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/4d91bce2-089e-4d91-9a21-9cd670c290c9" />
4. Challenge berhasil diselesaikan
   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/1fa00444-e978-4cdb-a91b-094a04a246bf" />

