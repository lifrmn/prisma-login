 LAPORAN PROYEK TUGAS FINAL

 
 📜 Pendahuluan.
Proyek ini merupakan tugas akhir yang bertujuan untuk membangun aplikasi web berbasis Node.js, Express.js, dan Prisma. Aplikasi ini digunakan untuk mengelola autentikasi pengguna serta menyediakan fitur-fitur yang mendukung pengelolaan data dengan Prisma ORM. Proyek ini juga mendukung deployment menggunakan Docker, sehingga memudahkan dalam proses deployment dan pengelolaan lingkungan aplikasi.


📖 1. Pengertian Proyek
Proyek ini adalah aplikasi web berbasis Node.js, Express.js, dan Prisma untuk mengelola autentikasi pengguna. Proyek ini menggunakan Prisma ORM untuk menghubungkan aplikasi dengan database, serta mendukung deployment dengan Docker.


![image](https://github.com/user-attachments/assets/e9fbc239-ccd1-4798-916c-32efc04cc9b3)


🖥️ server.js → Berisi kode server backend menggunakan Express.js.

🗄️ prisma/ → Direktori untuk ORM Prisma, digunakan untuk mengelola database.

🎨 public/ → Direktori untuk file frontend (HTML, CSS, dan JavaScript).

📦 Dockerfile → Konfigurasi untuk menjalankan aplikasi menggunakan Docker.

🔑 .env → Berisi konfigurasi database dan JWT_SECRET.

📜 package.json → Daftar dependensi dan skrip untuk menjalankan aplikasi.

CARA MENAJALANKAN 
JIKA TIDAK WORDSPACE BARU MAKA
1.npm start maka 🌐 http://localhost:3001
![Screenshot 2025-02-17 205503](https://github.com/user-attachments/assets/d062a955-7bcb-4ddf-a8f7-c4b4759e9c09)

jika membuat codespace baru:
1. npm install --legacy-peer-deps
![Screenshot 2025-02-18 193727](https://github.com/user-attachments/assets/e49c98f0-25d5-4852-baca-ae76b2163b46)
2.  npx prisma migrate dev
3. npm start
![Screenshot 2025-02-17 205503](https://github.com/user-attachments/assets/cacfdb26-27d1-47e9-94cc-15e7fbd05264)

Menjalankan dengan Docker
1. pastikn docker terinstal :docker -v
2. Bangun image Docker untuk aplikasi ini.: docker build -t tugas-final-lifrmn .
3. jalakan docker :docker run -p 3001:3001 tugas-final-lifrmn
4. 🌐 http://localhost:3001
   ![Screenshot 2025-02-18 210427](https://github.com/user-attachments/assets/0e07360f-5ea2-46cb-ba19-4f73d1a886b8)


![Screenshot 2025-02-18 210547](https://github.com/user-attachments/assets/ed76d8bf-cc7f-4e8d-91f0-167f57d96f42)


CARA BUKA DATA BASE :CODE = npx prisma Studio
![Screenshot 2025-02-17 170234](https://github.com/user-attachments/assets/2598a4bf-3b34-4a6d-a8d8-3e77c8238885)




 SERVER TIDAK BERJALAN UNTUK NPM
-Server Tidak Berjalan (``** gagal)**
   1.lsof -i :3001  # Untuk Linux/Mac
   2.kill -9 <PID>
   3.netstat -ano | findstr :3001  # Untuk Windows
   4.taskkill /PID <PID> /F
-Eror prisma generate
1.npx prisma migrate reset














-Container Docker Tidak Berjalan
1.docker ps -a
2.docker stop <CONTAINER_ID>
3.docker rm <CONTAINER_ID>
4.docker build -t tugas-final-lifrmn .
5.docker run -p 3001:3001 tugas-final-lifrmn


   












