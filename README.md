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
- Latar belakang dilakukannya analisa data ini adalah adanya sebuah artikel yang menyatakan bahwa terdapat lonjakkan insiden pembunuhan sebesar 54% pada tahun 2020 atau sebanyak 57 kasus dibandingkan dengan tahun sebelumnya yang hanya terjadi 37 insiden, dimana jumlah ini menjadi yang terkecil dalam 20 tahun terakhir.

Slide 7
![Problem_Statements](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_7.png)
- Berikut ini merupakan pernyataan masalah yang dibuat untuk membantu dalam menganalisa data ini:
    1. Apa jenis pelanggaran yang paling banyak terjadi di Kota Boston dalam rentang tahun 2015-2018?
    2. Apa saja nama distrik beserta titik-titik lokasi yang paling rawan terjadi sebuah insiden di Kota Boston?
    3. Bagaimana trend insiden pembunuhan dan insiden yang melibatkan penembakan di kota Boston dalam rentang tahun 2015-2018?
    4. Pada hari apa saja insiden pelanggaran cenderung banyak terjadi di Kota Boston? 
    5. Apakah ada kecenderungan insiden pelanggaran lebih banyak terjadi pada malam hari?
    6. Apa jenis pelanggaran yang sering terjadi berdasarkan kategori masing-masing UCR Part? 

Slide 8
![Insights&Recommmendation](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_8.png)
- Pada tahap ini akan dilihat Insight apa saja yang bisa diperoleh dari analisa data. Dari Insight tersebut akan diberikan rekomendasi yang diharapkan bisa membantu dalam menyelesaikan permasalahan yang terjadi ataupun meningkatkan kinerja Insight tersebut jika sudah baik.

Slide 9
![I&R_1a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_9.png)
- Berikut ini merupakan 5 jenis insiden dengan jumlah dan persentase terbesar

Slide 10
![I&R_1b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_10.png)
- Jenis insiden yang paling banyak dilaporkan merupakan pemberian bantuan medis kepada orang sakit atau terluka, yaitu sebesar 18.783 insiden dengan persentase sebesar 5,89%.
- Rekomendasi pertama, sebaiknya setiap petugas patroli dibekali dengan pelatihan dasar terkait pertolongan pertama pada korban kecelakaan. Hal ini juga bertujuan untuk mengantisipasi keterlambatan tenaga medis di jalan.
- Kemudian pada setiap mobil patroli kepolisian sebaiknya dipersiapkan kotak P3K atau kotak pertolongan pertama agar bisa digunakan apabila terjadi kecelakaan.

Slide 11
![I&R_2a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_11.png)
- Berikut ini merupakan pemetaan dari Kota Boston yang dibagi menjadi 12 distrik. Dimana semakin gelap warna suatu distrik, maka semakin banyak juga insiden yang terjadi di wilayah distrik tersebut.
- Lalu terdapat juga 10 *pin point* berwarna biru yang menunjukkan 10 titik lokasi dengan total insiden terbanyak di Kota Boston.

Slide 12
![I&R_2b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_12.png)
- Dapat terlihat bahwa insiden yang paling banyak terjadi berada di Distrik Roxbury (B2) dengan tanda warna merah tua sebesar 49.939 insiden dan persentase sebesar 15,74%.
- Sedangkan jumlah insiden yang paling sedikit terjadi berada di Distrik Charlestown (A15) dengan tanda warna cream muda sebesar 6.505 insiden dan persentase sebesar 2,04%.
- Terdapat pula 4 titik lokasi dengan total insiden terbanyak yang berdekatan di 3 distrik yang berbeda, yaitu pada distrik Roxbury (B2), South Boston (C6), dan South End (D4)
- Rekomendasi yang sebaiknya dilaksanakan, yaitu menambah personel serta jadwal patroli yang lebih banyak untuk mengawasi 5 distrik dengan total insiden yang cukup besar di antara 35.000 sampai 49.000 insiden, yaitu pada distrik Roxbury (B2), Dorchester (C11), South End (D4), Downtown (A1), dan Mattapan (B3).
- Departemen Kepolisian Kota Boston (BPD) juga disarankan untuk membentuk satuan tugas khusus untuk menyelidiki apakah terdapat hubungan atau keterkaitan antara 4 titik lokasi dengan total insiden terbanyak yang berdekatan di 3 distrik berbeda. Apakah di area tersebut terdapat sebuah kelompok kriminal yang terorganisir atau hanya sekedar kebetulan berdekatan saja.

Slide 13
![I&R_3a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_13.png)
- Berikut ini merupakan pola trend dari total insiden pembunuhan dan penembakan yang terjadi di kota Boston dari tahun 2015-2018.

Slide 14
![I&R_3b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_14.png)
- Jumlah insiden penembakan dan pembunuhan cenderung fluktuatif dari tahun 2015 hingga 2018. Dimana pada tahun 2015 hingga 2017, jumlah insiden mengalami peningkatan dan pada tahun 2017 hingga 2018, jumlah insiden mengalami penurunan yang cukup drastis.
- Hal ini menunjukkan bahwa tindakan preventif dan represif terhadap penggunaan senjata api bisa dikatakan berhasil menekan angka kriminalitas penembakan sampai dengan 185 insiden.
- Pada tahun 2018 terdapat 33 kasus pembunuhan yang terjadi, dimana pada tahun 2020 terjadi lonjakkan angka sebesar 54% dari tahun sebelumnya, yaitu 37 insiden. Secara tidak langsung hal ini menunjukkan bahwa insiden dengan menggunakan senjata api juga ikut mengalami peningkatan.
- Rekomendasi kepada Departemen Kepolisian Kota Boston adalah untuk meninjau kembali strategi preventif dan represif yang sebelumnya sudah berhasil dilakukan pada tahun 2017 hingga 2018. Karena ada besar kemungkinan bahwa senjata ilegal kembali bisa didapatkan dengan mudah dan tingkat pengawasan terhadap anggota geng juga mengalami kelonggaran. Perang antar geng bisa menjadi salah satu faktor yang menyebabkan insiden pembunuhan ini kembali meningkat.

Slide 15
![I&R_4a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_15.png)
- Berikut ini merupakan proporsi hari dalam 1 minggu dari setiap insiden yang terjadi di kota Boston.

Slide 16
![I&R_4b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_16.png)
- Berdasarkan pie chart, dapat terlihat bahwa insiden pelanggaran di Kota Boston banyak terjadi pada hari Jumat dengan persentase sebesar 15,20%. Disusul oleh hari Rabu dan Kamis dengan persentase masing-masing sebesar 14,65% dan 14,62%.
- Hari Sabtu dan Minggu merupakan hari dengan insiden pelanggaran yang paling sedikit terjadi dengan persentase sebesar 14,05% dan 12,64%.
- Hal ini menunjukkan bahwa insiden pelanggaran di Kota Boston cenderung lebih banyak terjadi pada hari-hari biasa dibandingkan pada hari akhir pekan. 
- Departemen Kepolisian Kota Boston (BPD) disarankan untuk mengevaluasi kembali jadwal patroli personel kepolisian. Dimana aktivitas patroli pada hari Rabu, Kamis, dan Jumat seharusnya lebih diprioritaskan dibandingkan dengan hari Sabtu dan Minggu. Dengan menambahkan jadwal patroli yang lebih banyak pada hari-hari tersebut diharapkan dapat menekan jumlah insiden per hari nya dan dapat menciptakan rasa yang lebih aman bagi warga Kota Boston.

Slide 17
![I&R_5a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_17.png)
- Berikut ini merupakan hasil uji hipotesis dan analisa grafik untuk mengetahui apakah terdapat kecenderungan lebih banyak insiden terjadi pada malam hari.
Hasil hipotesis menunjukkan Tolak H0, berarti Insiden pelanggaran cenderung tidak terjadi lebih banyak 50% pada malam hari.

Slide 18
![I&R_5b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_18.png)
- Berdasarkan uji hipotesis dan grafik pie-chart sebelumnya, dapat terlihat bahwa proporsi insiden yang terjadi pada malam hari tidak lebih banyak dibandingkan pada proporsi siang hari. Hal ini dapat dipengaruhi oleh faktor aktivitas warga pada malam hari yang lebih sedikit dibandingkan dengan siang hari.
- Namun karena faktor aktivitas warga yang lebih sedikit pada malam hari itulah yang membuat pelaku mendapatkan kesempatan dalam melancarkan aksi kejahatannya. Seperti contoh insiden perampokan rumah, dimana sering terjadi pada malam hari dan banyak warga yang sudah tertidur lelap, hal tersebut dapat memberikan kesempatan yang lebih besar untuk pelaku dalam menjalankan aksinya tanpa ketahuan oleh pemilik rumah. 
- Meskipun proporsi insiden pada siang hari lebih banyak terjadi, namun pada malam hari proporsi insiden yang terjadi juga cukup besar dengan persentase 37,44%. Oleh karena itu, Departemen Kepolisian Kota Boston disarankan untuk memperbanyak personel dan rute patroli pada malam hari. Terutama patroli pada daerah-daerah rawan terjadi insiden kriminal seperti yang telah dijabarkan pada poin analisa nomor 2. 

Slide 19
![I&R_6a](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_19.png)
- Berikut ini merupakan urutan kategori UCR dengan jumlah insiden terbanyak, serta 3 jenis insiden dengan kejadian terbanyak dari masing-masing kategori UCR_Part.

Slide 20
![I&R_6b](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_20.png)

Slide 21
![I&R_6c](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_21.png)

Slide 22
![I&R_6d](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_22.png)
- Berdasarkan keseluruhan tabulasi persilangan dapat terlihat bahwa persentase insiden terbesar merupakan kategori UCR Part 3 dengan nilai 49,69% dan total 158.537 insiden.
- Insiden Uniform Crime Reporting (UCR) Part 1 yang paling banyak terjadi di Kota Boston adalah pencurian di dalam bangunan dengan nilai curian diatas 200 USD dengan persentase di atas 12%.
- Insiden Uniform Crime Reporting (UCR) Part 2 yang paling banyak terjadi di Kota Boston adalah aktivitas pengrusakan atau coret mencoret properti orang lain tanpa izin sang pemilik dengan persentase di atas 15%.
- Insiden Uniform Crime Reporting (UCR) Part 3 yang paling banyak terjadi merupakan pemberian bantuan medis kepada orang sakit atau terluka sebesar 11,85%.
- Insiden Uniform Crime Reporting (UCR) Other atau kategori lain-lain dengan persentase di atas 85% dari seluruh insiden yang terjadi di UCR type ini adalah pengembalian kendaraan bermotor oleh kepolisian yang telah dicuri di luar Kota Boston.
- Insiden Uniform Crime Reporting (UCR) N/A atau kategori tidak diketahui dengan persentase di atas 89% dari seluruh insiden yang terjadi pada UCR type ini adalah masuk ke dalam rumah orang lain tanpa seizin pemilik rumah.
- Berdasarkan [Website Wikipedia Mengenai Uniform Crime Reports](https://en.wikipedia.org/wiki/Uniform_Crime_Reports), pelanggaran pidana hanya dibagi ke dalam dua kelompok besar, yaitu Pelanggaran Part 1 dan Pelanggaran Part 2. Oleh karena itu, Departemen Kepolisian Kota Boston (BPD) sebaiknya mempertimbangkan kembali pengelompokan insiden-insiden yang terjadi di kotanya. Karena menurut referensi tersebut, FBI hanya mengkategorikan Uniform Crime Report (UCR) menjadi 2 bagian saja, yaitu UCR Part 1 dan UCR Part 2. Sedangkan Departemen Kepolisian Kota Boston (BPD) membagi kategori UCR ini menjadi 3 Part dan bahkan terdapat 2 kategori lain, yaitu Other dan yang tidak diketahui (N/A). 

Slide 23
![Conclusion](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_23.png)
- Pelatihan dasar mengenai pertolongan pertama harus diberikan kepada personil patroli polisi dan kotak P3K juga harus tersedia di setiap kendaraan patroli.
- Perlu dilakukan penambahan personel patroli polisi, jadwal dan rute patroli polisi, terutama pada hari Rabu, Kamis, dan Jumat, serta pada malam hari di distrik2 yang paling rawan terjadi insiden kriminal.
- Strategi preventif dan represif terhadap penggunaan senjata api harus ditinjau kembali karena pada tahun 2020 terjadi lonjakkan 54% insiden pembunuhan atau sebanyak 57 kasus dibanding tahun sebelumnya, yaitu 37 kasus. Dari tahun 2015 sampai 2018, insiden penembakan dan pembunuhan juga menunjukkan pola trend yang cenderung sama.
- Pengelompokan kategori UCR oleh Departemen Kepolisian Kota Boston perlu ditinjau kembali karena berdasarkan kategori resmi yang diterbitkan oleh FBI, UCR hanya dikategorikan menjadi dua kelompok utama, yaitu UCR Part 1 dan UCR Part 2.

Slide 24
![Thank_You](https://github.com/marbill21/Capstone-Project-Modul-2/blob/main/Images/Slide_24.png)
- Sekian presentasi analisa data Crime In Boston dari saya, atas waktu dan perhatian, Saya ucapkan terima kasih.





















