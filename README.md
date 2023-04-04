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
- Dalam dataset ini, kolom-kolom yang berada di dalamnya dapat dijabarkan sebagai berikut:
    - Kolom `INCIDENT_NUMBER` merupakan nomor unik untuk setiap insiden yang terjadi di Kota Boston. Sedangkan `OFFENSE_CODE` merupakan Kode untuk kelompok jenis pelanggaran. Kedua kolom ini kemudian dikombinasikan untuk menjadi Index data terbaru mewakili setiap insiden dan jenis pelanggaran yang terjadi di Kota Boston.
    - Offense Detail: terdiri atas kolom `OFFENSE_CODE` (Kode untuk kelompok jenis pelanggaran), `OFFENSE_CODE_GROUP` (Nama kelompok kode jenis pelanggaran), dan `OFFENSE_DESCRIPTION` (Deskripsi pelanggaran yang terjadi).
    - Incident Location: terdiri atas kolom `DISTRICT` (Kode distrik terjadinya suatu insiden), `DISTRICT_NAME` (Nama distrik terjadinya suatu insiden), dan `Location` (Koordinat (garis lintang, garis bujur) dari lokasi terjadinya suatu insiden).
    - Incident Details: terdiri atas kolom `DATE` (Tanggal terjadinya suatu insiden), `TIME` (waktu terjadinya suatu insiden), `SHOOTING` (N - Tidak terjadi insiden penembakan, Y - Terjadi insiden penembakan), dan `UCR_PART` (Ranking jenis pelanggaran paling serius per insiden).
    - Unutilized Column: kolom yang dieliminasi atau tidak dipakai. Terdiri atas kolom `REPORTING_AREA` (Kode area pelaporan suatu insiden) dan `STREET` (Nama jalan terjadinya suatu insiden). Kedua kolom ini tidak bisa dihubungkan dengan data pada kolom lain sehingga menjadi tidak relevan.

Slide 6
![Background](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_6.png)

Slide 7
![Problem_Statements](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_7.png)

Slide 8
![Insights&Recommmendation](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_8.png)

Slide 9
![I&R_1a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_9.png)

Slide 10
![I&R_1b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_10.png)

Slide 11
![I&R_2a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_11.png)

Slide 12
![I&R_2b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_12.png)

Slide 13
![I&R_3a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_13.png)

Slide 14
![I&R_3b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_14.png)

Slide 15
![I&R_4a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_15.png)

Slide 16
![I&R_4b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_16.png)

Slide 17
![I&R_5a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_17.png)

Slide 18
![I&R_5b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_18.png)

Slide 19
![I&R_6a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_19.png)

Slide 20
![I&R_6b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_20.png)

Slide 21
![I&R_6c](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_21.png)

Slide 22
![I&R_6d](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_22.png)

Slide 23
![Conclusion](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_23.png)

Slide 24
![Thank_You](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_24.png)























