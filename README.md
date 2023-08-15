# Resampling Methode From Scratch

### Latar Belakang

Resampling methods adalah teknik statistik yang digunakan untuk mengatasi masalah seperti variabilitas, overfitting, atau evaluasi kinerja model. Metode ini melibatkan pengulangan atau pemilihan ulang sampel dari dataset yang ada untuk tujuan tertentu, seperti validasi model atau estimasi distribusi.

Dalam analisis statistik dan pembelajaran mesin, data yang digunakan sering kali terbatas dan mungkin tidak mewakili populasi secara sempurna. Resampling methods muncul sebagai solusi untuk mengatasi keterbatasan ini dengan memanfaatkan ulang data yang ada dalam berbagai cara kreatif.

**Jenis-Jenis Resampling Methods:**

**1. Bootstrapping:** 

Bootstrapping adalah teknik di mana sampel acak diambil dengan penggantian dari dataset yang ada. Ini memungkinkan kita untuk memperoleh estimasi distribusi sampel dari suatu statistik tanpa harus mengandalkan asumsi tertentu tentang distribusi populasi. Metode ini berguna dalam menghitung interval kepercayaan atau ketidakpastian statistik.

**2. Cross-Validation:**

Cross-validation (validasi silang) adalah metode untuk membagi dataset menjadi subset pelatihan dan validasi secara berulang. Model dilatih pada subset pelatihan dan dievaluasi pada subset validasi. Jenis cross-validation yang umum termasuk k-fold cross-validation dan leave-one-out cross-validation. Ini membantu menghindari overfitting dan memberikan gambaran yang lebih baik tentang kinerja model pada data yang tidak terlihat sebelumnya.

**3. Resampling Oversampling dan Undersampling:** 

Dalam konteks klasifikasi, ketidakseimbangan kelas dapat menjadi masalah. Oversampling melibatkan pengulangan sampel dari kelas minoritas, sementara undersampling melibatkan penghapusan beberapa sampel dari kelas mayoritas. Tujuannya adalah untuk mencapai keseimbangan antara kelas sehingga model tidak cenderung condong pada kelas mayoritas.

**Manfaat Resampling Methods:**

- Memungkinkan evaluasi model yang lebih akurat dengan memanfaatkan data yang ada secara efisien.
- Menghindari overfitting dan memperoleh estimasi ketidakpastian yang lebih baik.
- Berguna dalam menghadapi masalah seperti kelas yang tidak seimbang atau ketidakpastian statistik.
- Dapat membantu mengidentifikasi observasi yang memiliki pengaruh besar pada hasil.

Namun, perlu diingat bahwa setiap metode resampling memiliki batasan dan asumsi tersendiri, dan penerapannya harus disesuaikan dengan tujuan analisis dan karakteristik data yang sedang ditangani.

### Kelebihan Resampling Methods:

**1. Penggunaan Data yang Efisien:** 

Resampling methods memanfaatkan data yang ada secara lebih efisien. Dalam situasi di mana data terbatas, resampling memungkinkan kita untuk mendapatkan lebih banyak informasi dari dataset yang ada.

**2. Evaluasi Model yang Lebih Akurat:** 

Dengan membagi data menjadi subset pelatihan dan validasi berulang kali melalui cross-validation, resampling methods membantu menghindari overfitting dan memberikan estimasi kinerja model yang lebih akurat pada data yang tidak terlihat sebelumnya.

**3. Estimasi Ketidakpastian yang Lebih Baik:**

Resampling methods, seperti bootstrapping, membantu menghasilkan estimasi interval kepercayaan dan distribusi statistik yang lebih baik tanpa harus mengandalkan asumsi distribusi tertentu.

**4. Penanganan Ketidakseimbangan Kelas:**

Dalam klasifikasi, resampling methods seperti oversampling dan undersampling membantu menangani masalah kelas yang tidak seimbang dengan menciptakan keseimbangan yang lebih baik antara kelas-kelas yang berbeda.

**5. Identifikasi Pengaruh Observasi:**

Beberapa resampling methods, seperti jackknife, membantu mengidentifikasi observasi yang memiliki pengaruh besar terhadap hasil atau estimasi tertentu. Ini dapat membantu mengidentifikasi outlier atau pengamatan yang ekstrem.

### Kelemahan Resampling Methods:

**1. Komputasi yang Memakan Waktu:**

Beberapa metode resampling, terutama cross-validation dengan lipatan yang besar atau bootstrapping dengan banyak iterasi, dapat memakan waktu yang signifikan dalam perhitungan.

**2. Ketergantungan pada Pemilihan Parameter:**

Beberapa metode resampling memiliki parameter yang harus dipilih, seperti jumlah lipatan dalam k-fold cross-validation atau jumlah iterasi dalam bootstrapping. Pemilihan parameter yang tidak tepat dapat mempengaruhi hasil evaluasi.

**3. Risiko Overfitting Kecil:**

Meskipun resampling methods membantu menghindari overfitting, dalam beberapa kasus, mereka juga dapat memberikan perkiraan kinerja model yang terlalu optimis karena model dapat terbiasa dengan data yang diulang-ulang.

**4. Kemungkinan Informasi Kecil:**

Dalam metode seperti undersampling, informasi yang ada dalam kelas mayoritas mungkin hilang karena sebagian besar sampel dihilangkan. Ini dapat mengurangi kemampuan model untuk mengenali pola dalam kelas mayoritas.

**5. Sensitivitas terhadap Ketergantungan Data:**

Beberapa resampling methods, terutama bootstrapping, dapat menjadi sensitif terhadap ketergantungan data. Jika ada pengamatan yang sangat bergantung pada observasi lainnya, hasil resampling dapat terpengaruh.

**6. Tidak Membantu Dalam Mendapatkan Data Baru:**

Resampling methods tidak menciptakan data baru. Ini berarti bahwa jika data yang ada memiliki keterbatasan atau cacat, resampling methods tidak dapat memperbaiki masalah ini.

Pemilihan resampling method harus disesuaikan dengan tujuan analisis dan karakteristik data yang sedang ditangani. Setiap kelebihan dan kelemahan harus dievaluasi dengan cermat untuk memastikan penggunaan metode yang tepat dan interpretasi yang akurat dari hasil yang diperoleh.
