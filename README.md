QWEERTY Hotspot - Data Collection Form

📋 Deskripsi Proyek
QWEERTY Hotspot adalah halaman web sederhana berbasis HTML, CSS, dan JavaScript yang berfungsi untuk mengumpulkan data pengguna melalui form, 
kemudian mengirimkan informasi tersebut ke sebuah Discord webhook menggunakan Webhook API Discord.

Form ini menangkap informasi seperti:
- Nama lengkap
- Alamat email
- Tanggal lahir
- Gender (Jenis kelamin)
  
Setelah data diisi dan tombol Submit ditekan, data akan dikirimkan secara otomatis ke channel Discord yang telah dihubungkan melalui webhook.

🔧 Teknologi yang Digunakan
HTML5

- CSS3 (dalam file nr.css)
- JavaScript (vanilla)
- Discord Webhook API

📬 Cara Kerja Webhook

1. Form Submission:
Saat pengguna menekan tombol "Submit", fungsi JavaScript sendMessage() akan dipanggil.
Data dari input field (name, email, date, dan gender) diambil menggunakan document.getElementById dan querySelector.

2. Pengiriman Data ke Discord:
Data diformat menjadi sebuah string (contents) dan dikirim menggunakan XMLHttpRequest.
Webhook Discord menerima data ini dan mempostingnya sebagai pesan ke dalam channel Discord yang ditautkan.

3. Menutup Halaman:
Setelah 2 detik, halaman otomatis tertutup dengan window.close().

⚠️ Catatan Keamanan & Etika

⚠️ PENTING: Webhook ini secara aktif mengirim data personal ke sebuah endpoint Discord. Harap pastikan Anda:
- Memiliki izin yang sah untuk mengumpulkan data pengguna.
- Tidak menyalahgunakan webhook untuk keperluan phising, spam, atau aktivitas ilegal lainnya.
- Tidak menyebarkan data pribadi tanpa izin eksplisit dari pemilik data.

Jika digunakan dalam produksi, sangat disarankan untuk:
- Mengamankan endpoint webhook Anda (misalnya, menggunakan backend proxy).
- Menambahkan validasi data dan CAPTCHA.
- Menghindari pencatatan data sensitif jika tidak diperlukan.

🛠 Struktur Folder

📁 project-folder/
├── index.html
├── nr.css
└── README.md

📦 Contoh Output di Discord
Setelah form dikirim, isi webhook yang muncul di Discord:

 name: Benjamin
 email: Benja.min@example.com
 date: 2000-01-01
 gender: male
 
==================================

📄 Lisensi
© copyright@hrms.101
Proyek ini bersifat edukatif dan tidak diperuntukkan untuk penggunaan komersial tanpa izin.
