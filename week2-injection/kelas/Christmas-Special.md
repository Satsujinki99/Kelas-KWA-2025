# Chrismast Special

## Resource Belajar
https://www.invicti.com/blog/web-security/sql-injection-cheat-sheet/

1. Setelah menyelesaikan challenge ``database schema`` seperti yang kita ketahui bahwa juice shop memiliki vulnerability pada endpoint ''http://localhost:3000/#/rest/products/search?q=''

2. Anda bisa mencari produk yang ada namun dihapus pada lama juice shop dengan payload ini ``test')) UNION SELECT * FROM products WHERE deletedAt IS NOT NULL--``. Sama dengan soal ``database schema`` anda hanya perlu intercept laman saat mencari product lalu ubah bagian urlnya.
   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/af21d070-ab3c-4630-a34d-24227601c9e3" />
   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/d2c40eca-f182-4298-9902-bf7685e4119a" />

3. Coba untuk add produk apa saja ke basket, lalu send ke repeater, karena saya gagal terus pakai burpsuite jadi saya ngide pakai postman agar berhasil.
   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/219e49d0-1b18-4950-8f0e-ab5ee501752a" />
<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/7285afd7-e3a2-48ee-9928-9997a7ff1704" />
<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/1deb2804-dc27-4600-aa10-336c692699f8" />


