# A Deep Learning Project for Creating Line Art Potraits

<p>Ini merupakan projek dengan tujuan untuk membuat potrait seni garis atau Line Art Potraits yang menakjubkan. Model dirancang untuk mengambil gambar potret dan instruksi tertulis yang sesuai, lalu menggunakan instruksi tersebut untuk menyesuaikan gaya gambar. </p>

<h2>Line Art</h2>
<p>Hasil menakjubkan yang dihasilkan model ini memiliki resep rahasia tersendiri. Model awal tidak dapat membuat jenis output yang pemilik harapkan, model ini sebagian besar kesulitan mengenali fitur wajah. Meskipun ( https://github.com/yiranran/APDrawingGAN ) menghasilkan hasil yang bagus, model ini memiliki keterbatasan seperti (foto wajah depan mirip dengan foto ID, sebaiknya dengan fitur wajah yang jelas, tidak berkacamata, dan tidak berponi panjang.) Pemilik mencobanya dan menghasilkan hasil yang dapat mengenali pose apa pun. Mendapatkan garis yang tepat di sekitar wajah, mata, bibir, dan hidung bergantung pada data yang Anda berikan kepada model. Dataset APDrawing saja tidak cukup, jadi saya harus menggabungkan foto-foto terpilih dari dataset pasangan pewarnaan sketsa Anime. Dataset gabungan membantu model mempelajari garis dengan lebih baik.</p>

<h2>Technical Details</h2>
<ul>
  <li>Self-Attention ( https://arxiv.org/abs/1805.08318 ). Generator adalah UNET yang telah dilatih sebelumnya dengan normalisasi spektral dan self-attention. Sesuatu yang pemilik projek dapatkan dari DeOldify milik Jason Antic ( https://github.com/jantic/DeOldify ), ini membuat perbedaan besar, tiba-tiba pemilik projek mendapatkan detail yang tepat di sekitar fitur wajah.</li>
  <li>Progressive Resizing ( https://arxiv.org/abs/1710.10196),(https://arxiv.org/pdf/1707.02921.pdf ). Pengubahan ukuran progresif menggunakan ide untuk meningkatkan ukuran gambar secara bertahap. Dalam proyek ini, ukuran gambar ditingkatkan secara bertahap dan kecepatan pembelajaran disesuaikan. Terima kasih kepada fast.ai yang telah memperkenalkan pemilik projek pada pengubahan ukuran progresif, ini membantu model untuk menggeneralisasi lebih baik karena melihat lebih banyak gambar yang berbeda.</li>
  <li>Generator Loss Kehilangan Persepsi/Kehilangan Fitur berdasarkan VGG16. ( https://arxiv.org/pdf/1603.08155.pdf ).</li>
</ul>

<h2>Dataset</h2>
<p>[APDrawing dataset](https://cg.cs.tsinghua.edu.cn/people/~Yongjin/APDrawingDB.zip)

Kumpulan data pasangan pewarnaan sketsa anime

Kumpulan data APDrawing sebagian besar terdiri dari potret jarak dekat sehingga model akan kesulitan mengenali pakaian, tangan, dll. Untuk tujuan ini, gambar terpilih dari pasangan pewarnaan sketsa anime digunakan.</p>
