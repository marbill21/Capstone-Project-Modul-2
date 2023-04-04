# Capstone-Project-Modul-2
Nama : Mario Billy Gunawan <br>
Student ID : JCDSOL-009-022 <br>
Topik : [Crime in Boston](https://www.kaggle.com/datasets/AnalyzeBoston/crimes-in-boston) 
<hr>

## Project Guideline
Pada Module 2: Data Analysis, siswa telah mempelajari materi SQL, data manipulation,
data visualization, dan statistics. Capstone Project Module 2 ini bertujuan untuk
mengimplementasikan materi yang telah dipelajari oleh siswa dalam sebuah project.
Pengerjaan Capstone Project Module 2 ini diharapkan mampu melatih siswa dalam
membuat sebuah rangkaian analisis. Dalam projek ini, siswa akan memposisikan diri
sebagai data analyst dalam sebuah perusahaan. Siswa akan membuat serangkaian
pertanyaan sesuai berdasarkan keperluan bisnis dan masalah yang mungkin dihadapi oleh
perusahaan terkait sesuai dengan data yang didapatkan.

Siswa akan menjawab pertanyaan yang telah dibuat melalui analisis data, membuat cerita
dan visualisasi, serta mempresentasikan insight dari analisis yang kemudian bisa digunakan
stakeholders sebagai dasar pengambilan keputusan bisnis.

Pada akhir pengerjaan project, siswa wajib mengumpulkan 3 files, yaitu analisis yang
didokumentasikan dalam file Jupyter Notebook, story yang dibuat pada Tableau Public, dan
1 video yang menjelaskan permasalahan dan analisis yang dilakukan.

<hr>

## Project Presentation
Slide 1
![Crime_in_Boston](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_1.png)
- Topik yang saya dapatkan untuk mengerjakan Capstone Project Modul 2 ini adalah Crime in Boston <br>

Slide 2
![Table_of_Contents](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_2.png)
- Daftar isi dari presentasi ini diawali dengan mengidentifikasi profile data, merumuskan masalah, menjabarkan Insight dan Rekomendasi, dan terakhir menarik kesimpulan dari analisa data ini.

Slide 3
![Involved_Parties](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_3.png)
- Di dalam analisa data ini terdapat 2 pihak yang terlibat, pertama yaitu Saya Mario Billy Gunawan sebagai Konsultan Data Analis dan pihak kedua yaitu *Boston Police Department* sebagai *User* atau Klien.

Slide 4
![Data_Profile](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_4.png)
- Dataset yang digunakan pada analisa data ini terdiri dari 2, yaitu crime.csv dan offense_codes.csv
- Rentang waktu pengambilan data ini adalah dimulai dari tanggal 14 Juni 2015 sampai 3 September 2018.
- Lokasi pengambilan data ini adalah di Kota Boston, Negara Bagian Massachusetts, Amerika Serikat.
- Sumber dataset adalah berasal dari website Kaggle.com

Slide 5
![Columns](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_5.png)
- Dalam dataset ini, kolom-kolom yang terdapat didalamnya dapat dijabarkan sebagai berikut:
    - Kolom `Incident Number`: merupakan angka unik untuk setiap insiden, namun nomor yang sama akan dipakai untuk merepresentasikan beberapa respon polisi di dalam 1 kejadian. Maka, `Incident Number` digabung dengan `Offense Code` sehingga setiap angka unik dari kombinasi ini akan merepresentasikan 1 respon spesifik dari polisi terhadap 1 kejadian spesifik di lapangan.
    - Kategori Offense Code: dijabarkan melalui kolom `Code` (kode unik untuk setiap jenis respon polisi), `Name` (deskripsi singkat), `Group` (kategori tipe tindak kriminal yang terjadi), dan `Description` (deskripsi lengkap).
    - Kategori Crime Location: dijabarkan melalui kolom `District` yang berisi kode distrik. Kolom ini kemudian menjadi basis ditambahkannya kolom sintetis untuk menampung nama distrik dari setiap nomor distrik. Kemudian, ada angka unik berupa `Reporting Area` dan `Street Name` yang sulit untuk dikaitkan dengan kolom lainnya. Selain itu, dengan adanya kolom `Location` beserta kolom `Longitude` dan `Latitude` yang bisa langsung menunjukkan secara spesifik lokasi insiden di peta, maka relevansi kolom `Reporting Area` dan `Street Name` pun berkurang dan menyebabkan kolom ini tidak digunakan untuk analisa.
    - Kategori Crime Details: berisi inti dari dipakainya sistem pencatatan ini oleh polisi, yaitu untuk mencatat waktu secara lengkap dari tanggal, bulan, tahun, jam, menit, dan detik dari setiap pelaporan. Kemudian ada juga kolom `Shooting` yang mengindikasikan apakah terjadi penembakan dalam insiden tersebut. Lalu ada pula kolom Uniform Crime Reporting (UCR) Part yang mengkategorisasi setiap tindakan polisi kepada 4 Part yang berbeda dan akan dilaporkan kepada satuan keamanan yang berbeda.


https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_6.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_7.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_8.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_9.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_10.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_11.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_12.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_13.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_14.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_15.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_16.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_17.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_18.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_19.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_20.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_21.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_22.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_23.png

https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_24.png























