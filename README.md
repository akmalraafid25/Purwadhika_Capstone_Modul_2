# **Airbnb Listings Bangkok**
Dibuat oleh: *Akmal Raafid Taufiqurrahman*
- **Sumber Data: https://drive.google.com/drive/folders/1A_KBMRFTS5Mthpp46nulso679ML4ZwTF**

## **Content**

* **Data Understanding**
* **Exploratory Data Analysis**
* **Data Manipulation & Preprocessing**
* **Data Analysis**
    * Listing Analysis
        * Non-Luxury Listing
        * Luxury Listing Included
    * Host Analysis

## **Business Understanding**

### **Latar Belakang**
Airbnb merupakan salah satu platform penyewaan properti jangka pendek yang sangat populer, terutama di kota-kota besar seperti Bangkok. Dengan ribuan listing yang tersedia, kompetisi antara pemilik properti semakin tinggi. Oleh karena itu, pemilik properti maupun calon investor perlu memahami bagaimana faktor-faktor seperti harga, lokasi, ketersediaan, dan ulasan memengaruhi tingkat hunian dan pendapatan dari properti mereka.

Airbnb memperoleh keuntungan utamanya melalui biaya layanan yang dikenakan pada setiap transaksi antara tamu dan tuan rumah. Saat seorang tamu memesan akomodasi, Airbnb mengenakan biaya layanan sekitar 5% hingga 15% dari subtotal pemesanan, tergantung pada berbagai faktor seperti lokasi dan lama menginap. Di sisi lain, tuan rumah juga dikenakan biaya layanan oleh Airbnb, biasanya sekitar 3% dari subtotal pemesanan. Selain layanan akomodasi, Airbnb juga menawarkan produk tambahan seperti Airbnb Experiences, yaitu pengalaman lokal yang dikurasi, di mana perusahaan juga mengambil komisi dari setiap transaksi, bahkan hingga 20% dalam beberapa kasus. Meskipun tidak sebesar biaya layanan, Airbnb juga mendapatkan pendapatan dari fitur promosi berbayar bagi tuan rumah yang ingin meningkatkan visibilitas properti mereka di platform. Seluruh model bisnis Airbnb berlandaskan pada sistem platform digital yang menghubungkan pihak penyewa dan pemilik properti tanpa harus memiliki aset properti sendiri, menjadikannya perusahaan berbasis teknologi dengan margin operasional yang tinggi.

Dalam satu dekade terakhir, platform penyewaan jangka pendek seperti Airbnb telah mengubah cara orang memesan akomodasi dan cara individu memperoleh pendapatan dari properti mereka. Di kota-kota besar seperti Bangkok, yang merupakan salah satu destinasi wisata paling populer di dunia, Airbnb telah menjadi pilihan utama baik bagi wisatawan lokal maupun internasional.

Dengan meningkatnya jumlah listing dari tahun ke tahun, persaingan antar pemilik properti semakin ketat. Tidak hanya sekadar menyediakan tempat menginap, para host kini juga dituntut untuk menetapkan harga kompetitif, meningkatkan visibilitas, serta menjaga kualitas layanan agar tetap relevan di pasar. Di sisi lain, calon investor juga melihat Airbnb sebagai peluang usaha yang menjanjikan, terutama di lokasi-lokasi strategis dengan tingkat hunian tinggi.

Namun, tantangan yang muncul adalah bagaimana memahami faktor-faktor yang berpengaruh terhadap tingkat keberhasilan sebuah listing. Faktor seperti jenis kamar, lokasi geografis, jumlah ulasan, ketersediaan properti, serta harga memiliki kontribusi signifikan terhadap daya tarik listing tersebut. Tanpa pemahaman yang tepat berbasis data, keputusan bisnis yang diambil bisa kurang efektif dan berisiko menurunkan potensi pendapatan.

Melalui analisis data listing Airbnb di Bangkok, pelaku bisnis dapat memperoleh wawasan yang berguna untuk mengambil keputusan strategis, seperti penetapan harga yang optimal, pemilihan lokasi investasi, serta perencanaan promosi yang tepat sasaran.

Referensi:

Airbnb Help Center. (n.d.). What are Airbnb service fees? https://www.airbnb.com/help/article/104

Airbnb Investor Relations. (2023). Q4 2023 Financial Results. https://investors.airbnb.com

Investopedia. (2023). How Does Airbnb Make Money? https://www.investopedia.com/articles/investing/052615/how-does-airbnb-make-money.asp

### **Permasalahan Bisnis**

Berikut adalah beberapa pertanyaan bisnis yang dapat dijadikan acuan untuk analisis dataset ini:

* Bagaimana lokasi mempengaruhi **popularitas listing** di Bangkok?
* Bagaimana perbedaan harga antar **distrik**?
* Bagaimana **reviews** mempengaruhi *demand* suatu listing?
* Bagaimana **reviews** mempengaruhi performa host?
* Lokasi mana saja yang menjadi populer dari segi permintaan?

### **Tujuan Analisis (Goals)**

- Mengidentifikasi pengaruh lokasi terhadap popularitas listing di Bangkok untuk mengetahui area yang paling diminati oleh pemesan.

- Menganalisis perbedaan harga antar distrik guna memahami tren harga berdasarkan wilayah geografis.

- Mengevaluasi dampak ulasan (reviews) terhadap tingkat permintaan (demand) sebuah listing, dengan tujuan memberikan insight kepada host dalam meningkatkan daya tarik listing mereka.

- Menilai hubungan antara ulasan dan performa host untuk mengidentifikasi faktor-faktor review yang berkorelasi dengan host yang sukses.

- Menentukan lokasi-lokasi populer berdasarkan tingkat permintaan, sebagai referensi strategis dalam menentukan lokasi listing baru atau investasi properti.

### **Ekspektasi Hasil**

Harapannya pada analisis ini dapat diperoleh insights yang berpengaruh terhadap keputusan strategis, seperti penetapan harga yang optimal, pemilihan lokasi investasi, perencanaan promosi yang tepat sasaran juga actionable recommendation yang strategis.

### **Conclusion & Recommendation**

**Conclusion**

Berdasarkan analisis yang telah dilakukan berdasarkan beberapa pendekatan terhadap `listing`, untuk meninjau lebih jauh karakteristik listing yang bertujuan untuk memberikan insight dan rekomendasi, berikut adalah rangkuman kesimpulan dari analisis yang telah dilakukan:

* Lokasi memiliki pengaruh terhadap jumlah booking dan banyaknya listing. Hal ini menjadikan persaingan yang ketat. 
* Lokasi memiliki pengaruh terhadap harga. Lokasi yang memiliki akses transportasi publik yang baik dan dekat dengan tempat rekreasi cenderung menaikan standar harga listing di lokasi tersebut.
* Banyak Listing yang memiliki harga dibawah median. Ini disebabkan oleh 
* Host yang memiliki jumlah listing yang banyak cenderung memiliki jumlah bookings yang banyak tetapi hal ini tidak menjadi faktor utama banyaknya booking.
* Listing berjenis kamar `Entire Home/Apt` paling sering dibooking. Hal ini menjelaskan bahwa jenis kamar berpengaruh terhadap ketersediaan kamar.
* Listing yang memiliki ulasan banyak cenderung memiliki jumlah bookings yang lebih besar namun ini bukan menjadi faktor utama.

Lalu, karakteristik listing yang banyak diminati adalah listing yang terdapat:

* Lokasi listing yang memiliki akses transportasi yang baik
* Dekat dengan area konsentrasi turis (tempat wisata/area komersil)
* Memiliki ulasan (meskipun tidak signifikan)
* Merupakan properti yang tergolong pada kategori `Entire home/apt`

**Recommendation**

1. **Pengaturan Harga yang Lebih Strategis**

    Airbnb bisa memberikan saran harga yang lebih strategis bagi host, dengan mempertimbangkan lokasi, fasilitas, dan standar harga pada area tersebut. Misalnya, untuk lokasi dengan banyak turis, saran harga bisa lebih tinggi, sementara untuk lokasi yang lebih jauh dari pusat wisata, saran harga bisa lebih kompetitif.

2. **Prioritaskan Listing dengan Ulasan Positif**

    Meskipun ulasan tidak menjadi faktor utama, Airbnb bisa mempertimbangkan untuk memberikan sorotan lebih pada listing yang memiliki ulasan positif. Menampilkan rating tinggi pada hasil pencarian dapat memberikan motivasi kepada host untuk lebih fokus pada kualitas pengalaman tamu mereka. Hal ini dapat dilakukan dengan membuat segmen atau container baru pada aplikasi dan web yang berisikan Listing yang sedang memiliki ulasan bagus atau sedang ramai dipesan beberapa waktu terakhir

3. **Tingkatkan Fitur Pencarian Lokasi Berbasis Kebutuhan Pemesan**

    Airbnb bisa menambahkan filter lokasi yang lebih spesifik, misalnya:

    * Listing yang dekat dengan pusat kota
    * Listing yang dekat tempat wisata
    * Listing yang memiliki akses mudah ke transportasi umum

4. **Prioritaskan Listing dengan Tipe Entire Home/Apt**

    Mengingat bahwa jenis kamar Entire Home/Apt lebih sering dibooking, Airbnb dapat menyoroti listing tersebut dalam hasil pencarian atau lebih menyoroti listing berjenis serupa pada aplikasi. Hal ini bisa memberikan motivasi kepada host untuk membuat listing berjenis kamar ini dan juga meningkatkan kemungkinan booking pada listing tersebut. Selain itu, Airbnb juga dapat mempromosikan kamar berjenis Entire Home/Apt kepada calon host agar calon host lebih tertarik untuk membuat listing yang berjenis Entire Home/apt.

5. **Prioritaskan Listing yang memiliki Lokasi Strategis**

    Melihat dari analisis yang telah dilakukan, Airbnb bisa merekomendasikan listing yang berlokasi dekat dengan tempat wisata populer. Hal ini memungkinkan menarik pemesan untuk memilih listing yang dekat dengan tempat wisata tujuan. Ini dapat dilakukan dengan membuat promosi dalam aplikasi atau web seperti memunculkan `Place of Interest` yang terletak di sekitar listing yang sedang dilihat oleh pemesan.
