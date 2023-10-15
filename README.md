# Capstone-Modul-2
## Mengenai Dataset
#### 
Airbnb merupakan platform online yang memfasilitasi penyewaan tempat tinggal di seluruh dunia. Terdapat berbagai tipe tempat tinggal, mulai dari rumah, apartemen, kamar, hingga villa yang dapat disewa sesuai preferensi para tamu. Airbnb sangat mudah ditemukan di berbagai kota dan negara, salah satunya di Bangkok, Thailand. Dataset ini mengungkapkan Airbnb Listing di Bangkok yang memberi detail mengenai tipe kamar, ulasan dari para tamu, persebaran penginapan di Bangkok. Pada dataset ini, ditemukan ulasan yang buruk atau tidak ada review sama sekali yang mengakibatkan kehilangan kepercayaan terhadap potensial tamu. Oleh karena itu, analisis ini akan memberikan gambaran bagi Airbnb Bangkok dalam memperbaiki kebijakan yang lebih baik bagi Airbnb Bangkok, penyewa/host, dan para tamu.
## Stakeholder
#### Host/Penyewa dan Tamu di Airbnb Bangkok
## Permasalahan dan Goals
####
- Permasalahan:
1. Tamu tidak memberikan ulasan setelah check-out
2. Kurangnya ulasan mengakibatkan host kesulitan untuk meningkatkan kualitas unit mereka
3. Ulasan buruk atau tidak ada ulasan dari tamu dapat merusak reputasi Airbnb dan kurangnya kepercayaan di kalangan calon tamu

- Goals:
1. Membantu host dalam mengidentifikasi peningkatan kualitas penawaran mereka
2. Kebijakan untuk mewajibkan tamu memberikan ulasan
3. Bertujuan untuk terus memperbaiki pengalaman bagi host/penyewa dan tamu di platform
 
- Insights: 
1. Top 5 Penginapan berdasarkan Distrik
2. Top 5 Distrik dengan Total Ulasan Terendah
3. Room Type dan Minimum Malam di  50  Distrik Bangkok
4. Distribusi Distrik berdasarkan Review Category
5. Distrik dengan Review Category
6. Host ID di Vadhana yang Memiliki Review Category 'Tidak Ada Review' dan 'Sangat Buruk'
7. Host ID di Ratchathewi yang Menerima Jumlah Ulasan Terendah (12 Bulan Terakhir)

Hasil dari analisis adalah untuk memberikan rekomendasi-rekomendasi potensial kebijakan dalam pengambilan keputusan bagi Airbnb Bangkok.
## Nama Kolom dan Deskripsi
| Nama Kolom                      | Deskripsi                                                                   |
|---------------------------------|-----------------------------------------------------------------------------|
| id                              | unique ID dari listing                                         |
| name                            | Nama penginapan dari listing                                               |
| host_id                         | unique ID untuk penyewa/host                           |
| host_name                       | Nama depan penyewa/host                                                        |
| neighbourhood                    | Kawasan yang ditentukan berdasarkan koordinat geografis                     |
| latitude                        | Koordinat geografis lintang dari penginapan                                |
| longitude                       | Koordinat geografis bujur dari penginapan                                  |
| room_type                       | Jenis kamar atau akomodasi yang ditawarkan                                 |
| price                           | Harga harian dalam mata uang lokal   (Baht)                                     |
| minimum_nights                  | Jumlah minimum malam yang dibutuhkan untuk pemesanan                        |
| number_of_reviews               | Total jumlah ulasan yang diterima penginapan                                |
| last_review                     | Tanggal ulasan terbaru                                                     |
| reviews_per_month                     | Ulasan yang diterima per bulan                                                     |
| calculated_host_listings_count  | Jumlah penawaran yang dimiliki penyewa di kota/daerah yang sama         |
| availability_365                | Ketersediaan penawaran dalam 365 hari mendatang                            |
| number_of_reviews_ltm           | Jumlah ulasan yang diterima penawaran dalam 12 bulan terakhir             |
## Conclusion dan Recommendations
#### Conclusion
Berikut merupakan kesimpulan dari insights dari Visual Studio Code dan Tableau, 
- Vadhana dan Ratchathewi merupakan distrik dengan penginapan terbanyak dan juga tidak mendapatkan review, yang mendapatkan ulasan  sangat buruk, dan ulasan terendah selama 12 bulan terakhir.

- Distrik Vadhana merupakan top 1 distrik dengan penginapan terbanyak di Bangkok tetapi memiliki review category 'Tidak Ada Review' dan 'Sangat Buruk'. Hal tersebut disebabkan oleh tamu yang tidak memiliki waktu akibat letak Vadhana yang strategis akan pusat perbelanjaan dan hiburan, khususnya Thonglor dan Ekamai. Para tamu lebih banyak mengalokasi waktu untuk mengeksplor Vadhana dibandingkan mengisi ulasan.

Untuk mengetahui penginapan mana saja di Vadhana yang memiliki total ulasan terendah selama 12 bulan, maka dicari berdasarkan host ID. Berikut merupakan 5 host ID terendah:
1. 485313876
2. 474260020
3. 465486937
4. 456119431
5. 449012324

- Distrik Ratchathewi merupakan top 4 distrik dengan penginapan terbanyak di Bangkok tetapi memiliki total ulasan terendah selama 12 bulan terakhir. Hal tersebut disebabkan oleh tamu yang tidak memiliki waktu setelah menginap karena Ratchathewi terletak di pusat kota dengan berbagai tempat yang menghibur. Yang terkenal dari distrik ini adalah MBK Center dan Siam Paragon. 

Untuk mengetahui penginapan mana saja di Ratchathewi yang memiliki total ulasan terendah selama 12 bulan, maka dicari berdasarkan host ID. Berikut merupakan 5 contoh host ID terendah:
1. 153793
2. 595560
3. 4117536
4. 5115355
5. 5357273

#### Recommendations:
1. Bagi Airbnb dan penyewa:
- Airbnb menghubungi penyewa yang memiliki unit dengan review 'sangat buruk' dan 'tidak ada review'. Hal tersebut dilakukan agar host meningkatkan kualitas unitnya. Apabila tidak dilaksanakan dalam waktu tertentu, maka Airbnb memiliki otoritas untuk memutuskan hubungan dengan host. Pihak Airbnb juga harus mengawasi setiap progress dari host terhadap unitnya.

2. Bagi tamu:
- Dengan tamu yang cenderung lupa akibat keterbatasan waktu, Airbnb dapat memberi pesan reminder melalui e-mail aplikasi dari guest setelah mereka menginap
- Dentan tamu yang cenderung tidak merasa untung, Airbnb dapat memberi benefit bagi tamu yang memberi ulasan, seperti sistem mengumpulkan poin yang dapat diredeem untuk penginapan selanjutnya
- Dengan tamu yang cenderung takut menjalin hubungan yang buruk dengan penyewa, tamu diberi sebuah penjelasan bahwa review harus ditulis secara jujur dan penyewa tidak mampu mengganggu gugat atas review tersebut
