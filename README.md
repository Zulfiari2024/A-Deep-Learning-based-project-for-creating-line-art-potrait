TL; DR Memahami pengklasifikasi spam atau ham dari aspek konsep Kecerdasan Buatan, bekerja dengan berbagai algoritma klasifikasi, dan memilih algoritma produksi akurasi tinggi dan mengembangkan Aplikasi Python Flask untuk SMS: spam atau detektor ham.
Layanan Pesan Singkat (SMS) jauh lebih dari sekadar teknologi untuk obrolan. Teknologi SMS berevolusi dari sistem global untuk standar komunikasi seluler, yang diterima secara internasional[1]. Spam adalah penyalahgunaan sistem pesan elektronik untuk mengirim pesan yang tidak diminta secara massal tanpa pandang bulu [2]. Sementara bentuk spam yang paling dikenal luas adalah spam email, istilah ini diterapkan pada penyalahgunaan serupa di media dan media lain. Spam SMS dalam konteksnya sangat mirip dengan spam email, biasanya, pesan massal yang tidak diminta dengan beberapa kepentingan bisnis. Spam SMS digunakan untuk iklan komersial dan menyebarkan tautan phishing. Spammer komersial menggunakan malware untuk mengirim spam SMS karena mengirim spam SMS adalah ilegal di sebagian besar negara. Mengirim spam dari mesin yang disusupi mengurangi risiko bagi spammer karena mengaburkan asal-usul spam.
Deteksi spam SMS adalah tugas penting di mana pesan SMS spam diidentifikasi dan disaring. Karena jumlah pesan SMS yang lebih signifikan dikomunikasikan setiap hari, sulit bagi pengguna untuk mengingat dan mengkorelasikan pesan SMS yang lebih baru yang diterima dalam konteks dengan SMS yang diterima sebelumnya. Dengan demikian, dengan menggunakan pengetahuan kecerdasan buatan dengan penggabungan pembelajaran mesin, dan penambangan data kami akan mencoba mengembangkan spam teks SMS berbasis web atau detektor ham.
Ini adalah tiga bagian dari seri blog, di mana kita akan memahami masuk dan keluar spam atau pengklasifikasi ham dari aspek konsep Kecerdasan Buatan, dan bekerja dengan berbagai algoritma klasifikasi di jupyter notebook dan memilih satu algoritma berdasarkan kriteria kinerja. Kemudian, kami akan mengembangkan spam teks SMS berbasis web Python atau detektor ham.

Apa yang akan kami bahas di sini

Konsep AI Teoretis Mengenai Pengklasifikasi Spam atau Ham
Algoritma Klasifikasi
Menjelajahi Sumber Data
Persiapan Data
Analisis Data Eksplorasi
Bayes Naif di Balik Spam atau Ham
Kriteria Pengukuran Kinerja
Pengembangan Detektor Spam atau Ham
Deskripsi Agen
Seperti yang telah disebutkan, kami akan membuat proyek ini dari aspek konsep kursus Kecerdasan Buatan, jadi, mari kita pahami agennya.

Karena proyek ini sederhana untuk dirancang yaitu, agen dapat mengklasifikasikan teks (pesan) yang masuk sebagai ham atau spam hanya berdasarkan jenis agen[6]; agen proyek ini berada di bawah agen refleks sederhana karena mengambil tindakan berdasarkan situasi lingkungan saat ini saja, yaitu, memetakan persepsi saat ini ke dalam tindakan yang tepat mengabaikan sejarah persepsi. 
