# DS-CAPSTONE2-AWS
Capstone 2 Data Science Purwadhika. Proyek ini berfokus pada pengolahan dan analisis data transaksi AWS SaaS untuk menghasilkan wawasan yang dapat ditindaklanjuti guna mengoptimalkan strategi penjualan.

[Link Dashboard dapat diakses di sini](https://lookerstudio.google.com/reporting/f0079418-edfe-49a1-b378-5338ca104855)

## AWS SaaS

**Software-as-a-Service (SaaS)** yang dibangun dan diterapkan di **Amazon Web Services (AWS)** dikenal sebagai AWS SaaS. Model pengiriman berbasis cloud ini menghosting aplikasi perangkat lunak pada infrastruktur AWS, menyediakan akses bagi pelanggan melalui internet tanpa memerlukan instalasi atau pemeliharaan lokal.

### Manfaat Utama AWS SaaS:
- **Jangkauan Global**: Infrastruktur global AWS memastikan pengiriman aplikasi SaaS dengan latensi rendah ke seluruh dunia.
- **Skalabilitas**: Memungkinkan penskalaan aplikasi dengan mudah untuk memenuhi permintaan yang berfluktuasi, menjaga performa dan keandalan.
- **Keamanan**: Fitur keamanan yang kuat seperti enkripsi, kontrol akses, dan deteksi ancaman melindungi aplikasi dan data pelanggan.
- **Efektivitas Biaya**: Model harga bayar sesuai penggunaan mengoptimalkan biaya berdasarkan penggunaan.
- **Produktivitas Pengembang**: Beragam alat dan layanan AWS mempercepat pengembangan dan penerapan aplikasi SaaS.

**Informasi lebih lanjut tentang bisnis**: [AWS SaaS](https://aws.amazon.com/saas/)

---

## Latar Belakang

AWS SaaS berperan penting dalam menyediakan layanan cloud yang skalabel dan efisien secara global. Untuk meningkatkan strategi bisnis dan pengambilan keputusan, analisis indikator kinerja utama (KPI) seperti **penjualan**, **jumlah terjual**, **margin keuntungan**, dan **diskon** sangat penting. Analisis ini didasarkan pada kebutuhan berikut:

1. **Lanskap Pasar yang Dinamis**  
   AWS SaaS beroperasi di pasar yang kompetitif dengan kemajuan teknologi cepat dan permintaan pelanggan yang beragam. Memahami **tren penjualan, jumlah, dan keuntungan** sangat penting untuk mengevaluasi kinerja bisnis dari waktu ke waktu.

2. **Wawasan Kinerja Produk**  
   Setiap produk AWS SaaS melayani kebutuhan pelanggan yang berbeda. Melacak **KPI spesifik produk** membantu mengidentifikasi produk unggulan dan mengatasi yang berkinerja rendah.

3. **Fokus Regional dan Industri**  
   Sebagai penyedia global, AWS SaaS memerlukan wawasan tentang **tren regional dan industri** untuk menyesuaikan strategi, mengalokasikan sumber daya secara efisien, dan menemukan peluang pertumbuhan baru.

4. **Tren Profitabilitas**  
   Memantau **rasio keuntungan terhadap penjualan** menunjukkan seberapa efektif penjualan dikonversi menjadi keuntungan, mengidentifikasi area untuk perbaikan operasional atau harga.

5. **Dampak Diskon**  
   Diskon mendorong penjualan namun dapat merugikan keuntungan. Menganalisis **korelasi antara diskon dan rasio keuntungan terhadap penjualan** memastikan keseimbangan antara pertumbuhan pendapatan dan profitabilitas.

Dengan mengatasi area-area ini, AWS SaaS dapat memperoleh wawasan yang dapat ditindaklanjuti untuk mendukung keputusan berbasis data, mendorong pertumbuhan berkelanjutan dan kepemimpinan pasar.

---

## Pernyataan Masalah

Analisis ini bertujuan menjawab pertanyaan berikut untuk mengoptimalkan strategi penjualan, khususnya di Q1:

1. **Bagaimana tren penjualan di berbagai industri (energi, teknologi, keuangan, ritel, dll.) dapat dimanfaatkan untuk mengoptimalkan strategi tim penjualan di awal tahun?**
2. **Produk mana yang berkinerja terbaik di setiap industri, dan bagaimana tim penjualan dapat memprioritaskannya untuk memaksimalkan profitabilitas?**
3. **Faktor apa (misalnya, diskon, segmen pelanggan, atau wilayah geografis) yang paling memengaruhi kinerja penjualan di Q1, dan bagaimana cara mengelolanya untuk meningkatkan efisiensi tim penjualan?**
4. **Bagaimana pola musiman, khususnya di Q1, memengaruhi penjualan di berbagai industri, dan strategi apa yang dapat memanfaatkan pola tersebut?**

---

## Tujuan

- **Mengidentifikasi tren penjualan berdasarkan industri** untuk menyusun strategi penjualan Q1 yang lebih efektif.
- **Menentukan produk unggulan per industri** untuk memandu tim penjualan dalam memprioritaskan upaya pemasaran dan penjualan guna meningkatkan profitabilitas.
- **Menganalisis faktor yang memengaruhi kinerja penjualan** (misalnya, diskon, segmen pelanggan, wilayah) untuk merancang pendekatan yang lebih terarah dan efisien.
- **Memahami pola musiman di Q1** untuk membuat rencana aksi yang memanfaatkan peluang pasar dan meminimalkan risiko.

Tujuan ini bertujuan meningkatkan kinerja tim penjualan di Q1, memperkuat posisi pasar, dan meletakkan dasar untuk mencapai target penjualan tahunan.

---

## Deskripsi Dataset

Dataset `SaaS-Sales.csv` berisi 9.994 catatan transaksi dengan kolom-kolom berikut:

| **Nama Kolom**     | **Deskripsi**                                           |
|---------------------|---------------------------------------------------------|
| **Row ID**         | Pengenal unik untuk setiap transaksi.                  |
| **Order ID**       | Pengenal unik untuk setiap pesanan.                    |
| **Order Date**     | Tanggal pesanan dibuat.                               |
| **Date Key**       | Representasi numerik tanggal (YYYYMMDD).              |
| **Contact Name**   | Nama individu yang membuat pesanan.                   |
| **Country**        | Negara tempat pesanan dibuat.                         |
| **City**           | Kota tempat pesanan dibuat.                           |
| **Region**         | Wilayah tempat pesanan dibuat.                        |
| **Subregion**      | Subwilayah tempat pesanan dibuat.                     |
| **Customer**       | Perusahaan yang membuat pesanan.                      |
| **Customer ID**    | Pengenal unik untuk setiap pelanggan.                 |
| **Industry**       | Industri pelanggan.                                   |
| **Segment**        | Segmen pelanggan (SMB, Strategic, Enterprise, dll.).  |
| **Product**        | Produk yang dipesan.                                  |
| **License**        | Kunci lisensi produk.                                 |
| **Sales**          | Total jumlah penjualan transaksi.                     |
| **Quantity**       | Jumlah item dalam transaksi.                          |
| **Discount**       | Diskon yang diterapkan pada transaksi.                |
| **Profit**         | Keuntungan dari transaksi.                            |

---

## Ringkasan Analisis

Analisis menggunakan pustaka Python (`pandas`, `numpy`, `matplotlib`, `seaborn`) untuk mengeksplorasi dataset dan menjawab pernyataan masalah. Temuan utama meliputi:

- **Tren Penjualan Q1**: Rata-rata penjualan Q1 ($88,697.89) lebih rendah dibandingkan kuartal lain ($161,867.44), menunjukkan perlunya strategi khusus untuk menangkap anggaran tahunan lebih awal.
- **Kinerja Industri**: **Keuangan** dan **Energi** mendominasi penjualan, dengan pertumbuhan signifikan dari 2020–2023. **Produk Konsumen** menunjukkan profitabilitas stabil, sementara **Transportasi** dan **Manufaktur** menghadapi tantangan.
- **Kinerja Produk**: **ChatBot Plugin**, **Support**, dan **Marketing Suite - Gold** unggul dalam volume transaksi dan profitabilitas, ideal untuk **Keuangan** dan **Energi**. **ContactMatcher** memerlukan pengelolaan diskon ketat karena tingkat diskon tinggi memengaruhi keuntungan.
- **Dampak Diskon**: Korelasi negatif antara diskon dan keuntungan menekankan perlunya membatasi diskon tinggi (misalnya, >0.50) untuk menjaga profitabilitas.
- **Pola Musiman**: Q1 menawarkan peluang di **Keuangan** dan **Energi** karena pembaruan kontrak, tetapi diskon tinggi dapat merusak keuntungan.

### Visualisasi Utama
- **Heatmap Korelasi**: Menunjukkan hubungan negatif antara diskon dan keuntungan.
- **Dashboard**: Visualisasi interaktif di Looker Studio memberikan wawasan mendetail tentang penjualan, keuntungan, dan kinerja produk berdasarkan industri dan wilayah.

---

## Kesimpulan dan Rekomendasi

### 1. **Mengoptimalkan Tren Penjualan berdasarkan Industri**
- **Wawasan**: **Keuangan** dan **Energi** memimpin penjualan Q1, didorong oleh alokasi anggaran tahunan. **Produk Konsumen** menawarkan profitabilitas stabil, sementara **Transportasi** kesulitan.
- **Rekomendasi**: Luncurkan kampanye Q1 agresif untuk **Keuangan** dan **Energi** guna menargetkan kontrak besar. Promosikan produk margin tinggi di **Produk Konsumen** dengan diskon minimal. Kurangi fokus pada **Transportasi** kecuali ada peluang dengan keuntungan tinggi.

### 2. **Memprioritaskan Produk Unggulan**
- **Wawasan**: **ChatBot Plugin**, **Support**, dan **Marketing Suite - Gold** unggul dalam volume dan profitabilitas, terutama di **Keuangan** dan **Energi**. **ContactMatcher** berisiko menurunkan keuntungan karena diskon tinggi.
- **Rekomendasi**: Prioritaskan **ChatBot Plugin** dan **Support** di **Keuangan** dan **Energi** dengan diskon rendah. Batasi diskon **ContactMatcher** hingga 0.20 di industri potensial. Tawarkan bundling **Marketing Suite - Gold** untuk **Produk Konsumen** guna meningkatkan penjualan.

### 3. **Mengelola Faktor yang Memengaruhi Penjualan Q1**
- **Wawasan**: Diskon sangat memengaruhi profitabilitas, dengan diskon tinggi (0.70–0.80) menyebabkan kerugian. **Keuangan** dan **Energi** (kemungkinan didominasi Enterprise) menunjukkan kinerja Q1 yang kuat, tetapi analisis geografis terbatas.
- **Rekomendasi**: Batasi diskon pada 0.20 untuk sebagian besar produk di Q1. Targetkan segmen Enterprise di **Keuangan** dan **Energi** dengan penawaran khusus. Fokuskan kampanye pada wilayah dengan penjualan tinggi (misalnya, EMEA, AMER) berdasarkan data historis.

### 4. **Memanfaatkan Pola Musiman Q1**
- **Wawasan**: Penjualan Q1 lebih rendah dibandingkan kuartal lain, tetapi **Keuangan** dan **Energi** tetap kuat karena pembaruan kontrak. Diskon tinggi di Q1 merusak profitabilitas di industri seperti **Manufaktur**.
- **Rekomendasi**: Luncurkan kampanye Januari–Februari untuk **Keuangan** dan **Energi** dengan uji coba gratis atau demo untuk **Support** dan **FinanceHub**. Hindari diskon agresif di **Transportasi** dan **Manufaktur**. Gunakan dashboard untuk melacak kinerja Q1 secara real-time.

### Penilaian Keseluruhan
Analisis berhasil menjawab pernyataan masalah, mengidentifikasi tren utama, produk unggulan, dampak diskon, dan peluang Q1. Meskipun analisis geografis dan segmen pelanggan kurang mendalam, rekomendasi sejalan dengan optimalisasi kinerja penjualan Q1, fokus pada industri dan produk berpotensi tinggi.

---

## 🚀 Tentang Saya
Muhammad Rikza Nauval Fachry, siswa Bootcamp Data Science Purwadhika 2025, On-Campus Jogja. Proyek ini menunjukkan kemampuan saya menganalisis dataset kompleks dan menghasilkan wawasan strategis untuk optimalisasi bisnis.

---

README ini disusun untuk memberikan gambaran jelas tentang analisis AWS SaaS, sejalan dengan konten dan tujuan notebook. Beri tahu saya jika ada penyempurnaan lebih lanjut yang diinginkan!
