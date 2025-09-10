# User-Credentials

## Resource Belajar

## Step by step
1. Pada challenge ini kita diminta mencari semua user credential, caranya mirip dengan ``database schema`` hanya saja payloadnya sedikit berbeda.
2. Seperti yang sudah saya paparkan pada challenge sebelumnya, endpoint `localhost:3000/rest/products/search?q=` memiliki vulnerability yang fatal, ki
hanya perlu payload ``M')) UNION SELECT id,email,password,4,5,6,7,8,9 FROM users--`` dan challenge berhasil diselesaikan

<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/b07dffa9-d422-4841-b067-9b55849bcc32" />
<img width="1439" height="856" alt="image" src="https://github.com/user-attachments/assets/e0574611-ec53-464b-999d-1ad3814a842d" />

