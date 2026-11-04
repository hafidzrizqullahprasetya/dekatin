# Product Requirements Document (PRD) — Dekat.in (MVP)

Dokumen ini merupakan spesifikasi kebutuhan produk untuk Minimum Viable Product (MVP) Dekat.in, yang disusun berdasarkan sintesis empat dokumen perancangan awal: Creative Thinking (02), Customer Discovery (03), Value Proposition Canvas & Business Model Canvas (04), serta Prioritas Fitur & MVP (05).

---

## 1. Ringkasan Produk & Value Proposition Statement

Dekat.in adalah platform etalase digital hyperlocal berbasis web yang menghubungkan pelaku UMKM mikro dan penjual rumahan (seperti produsen frozen food, katering harian, snack box, kue basah, hingga pengrajin buket) dengan calon pembeli di lingkungan pemukiman terdekat dalam radius mikro (<3–5 KM). Platform ini berfungsi murni sebagai instrumen penemuan lokal (discovery tool) tanpa keranjang belanja atau sistem pembayaran di dalam aplikasi (in-app checkout), melainkan mengalihkan transaksi secara langsung ke kanal obrolan WhatsApp penjual melalui mekanisme 1-click order dengan pesan terformat otomatis. Model ini mempertahankan 100% margin keuntungan pedagang (0% komisi transaksi) serta membebaskan pembeli dari beban biaya kurir instan pihak ketiga melalui opsi pemenuhan mandiri (ambil sendiri atau diantar langsung oleh pedagang).

### Value Proposition Statement
> "Platform etalase digital hyperlocal yang membantu penjual rumahan ditemukan oleh tetangga dan pembeli terdekat dalam radius 5 KM, serta bertransaksi langsung via WhatsApp tanpa potongan biaya komisi dan bebas dari mahalnya ongkos kirim." (Dikutip dari dokumen 04-vpc-bmc.md, Bagian 2).

---

## 2. Masalah & Target Pengguna

### 2.1. Rumusan Masalah
Pelaku UMKM mikro dan penjual rumahan kesulitan ditemukan oleh calon pembeli di radius tempat tinggal terdekatnya (<3–5 KM) karena keterbatasan jangkauan status chat dan algoritma media sosial yang tidak memprioritaskan lokasi mikro. Pilihan promosi berbayar tidak terjangkau bagi usaha bermargin tipis, sedangkan platform marketplace besar menenggelamkan toko baru di antara ribuan pesaing. Di sisi lain, pembeli lokal kesulitan menemukan alternatif produk rumahan segar di sekitarnya dan kerap membatalkan pesanan karena tarif kurir instan pihak ketiga lebih mahal daripada harga produk itu sendiri, ditambah beban komisi aplikasi pesan-antar konvensional (20%–30%).

### 2.2. Persona Pengguna

#### Persona Penjual (Versi Setelah Validasi Lapangan)
* **Nama Persona:** Ibu Rina (35 Tahun)
* **Peran/Kategori:** Penjual frozen food dan makanan rumahan
* **Karakteristik & Perilaku:** Melek teknologi namun sangat pragmatis. Mengoperasikan usaha secara mandiri menggunakan smartphone tanpa tim pemasaran dan tanpa komputer/laptop. Mengalami kelelahan akibat interaksi media sosial (likes/shares) yang tinggi namun tidak menghasilkan penjualan nyata karena terkendala mahalnya ongkos kirim antar-wilayah.
* **Kebutuhan Utama:** Etalase digital berbasis area lokal terdekat agar dapat ditemukan tetangga sekitar, tanpa proses pendaftaran atau dasbor inventaris yang rumit, serta dapat bertransaksi langsung via WhatsApp tanpa potongan biaya komisi.

#### Persona Pembeli (Diderivasi dari Temuan Responden Pembeli di Dokumen 03)
* **Kategori Pengguna:** Mahasiswa penghuni kos, pekerja WFH, pendatang baru, dan warga perumahan (direpresentasikan oleh responden Dimas, Mbak Linda, dan Arif).
* **Karakteristik & Perilaku:** Mengandalkan smartphone untuk mencari kebutuhan makanan harian, lauk siap masak, cemilan, atau layanan mendadak di sekitar tempat tinggal. Terbiasa dengan transaksi cepat via transfer bank, QRIS, atau uang tunai.
* **Kebutuhan Utama:** Informasi terpusat mengenai penjual produk rumahan terdekat dalam radius jalan kaki atau berkendara singkat, bebas biaya layanan aplikasi, bebas ongkos kirim mahal melalui opsi ambil sendiri (self-pickup) atau antar mandiri.

### 2.3. Kutipan Pernyataan Kunci Responden Wawancara Lapangan
Berikut 6 kutipan paling relevan dari hasil wawancara 10 responden pada dokumen 03-customer-discovery.md:
1. **Responden 1 — Bu Ningsih (44 tahun, Penjual Katering Rumahan dan Snack Box, Mlati, Sleman):**
   > "Kalau jualan makanan basah/snack box begini, pasarnya harus yang dekat-dekat aja mas, maksimal 5KM biar gak basi di jalan. Masalahnya warga perumahan sebelah aja banyak yang gak tahu saya jualan katering"
2. **Responden 3 — Mbak Sarah (27 tahun, Penjual Dessert Box dan Brownies Panggang, Depok, Sleman):**
   > "Mau daftar ojol makanan potongannya bikin pusing kalau jualan dari kos/rumah. Saya cuma posting status WA sama minta tolong teman repost. Kalau lagi gak ada yang di share, seharian bisa nol order."
3. **Responden 4 — Pak Dedi (49 tahun, Pengerajin Sambal Botol dan Keripik Tempe, Kasihan, Bantul):**
   > "Saya gapyek kalau harus ngisi dashboard toko online yang banyak formnya. yang penting buat saya itu orang tahu nomor WA saya, tahu dengan daganagan saya dimana, terus langsung chat WA"
4. **Responden 5 — Ibu Ratna (38 tahun, Penjual Frozen Food dan Dimsum Homemade, Ngaglik, Sleman):**
   > "Keluhan terbesar pembeli itu ongkir. Kemarin ada yang mau beli dimsum 30 ribu, pas cek ongkir instan ternyata 22 ribu karena beda kecamatan dan jauh. Akhirnya batal. Padahal kalau ada pembeli radius 2 km kan bisa saya anterin gratis pas sore"
5. **Responden 7 — Dimas (21 tahun, Pembeli / Mahasiswa Kos, Kaliurang KM 5):**
   > "Sering mager keluar cari makan atau jajanan ringan, taoi kalau buka aplikasi delivery kenanya mahal di ongkir plus biaya layanan. Padahal pengen tau tetangga kos atau gang sebelah ada jualan lau atau cemilan apa."
6. **Responden 8 — Mbak Linda (32 tahun, Pembeli / Ibu Rumah Tangga / WFH, Seturan, Sleman):**
   > "Saya lebih senang beli sayur potong siap masak atau lauk matang dari ibu-ibu rumahan sekitar. Lebih bersih dan fresh. Masalahnya saya cuma tahu dari mulut ke mulut, gak ada satu tempat yang ngerangkum jualan tetangga."

---

## 3. Prinsip Produk yang Tidak Boleh Dilanggar

Berdasarkan kesepakatan rancangan pada dokumen 02, 03, 04, dan 05, prinsip-prinsip berikut bersifat non-negotiable dan tidak boleh dilanggar dalam pengembangan Dekat.in:
1. **0% Komisi Transaksi (Zero Commission Fee):** Platform tidak memungut persentase komisi atau biaya admin apa pun dari nilai transaksi penjualan. 100% hasil penjualan menjadi hak utuh pedagang.
2. **Tanpa Payment Gateway & Tanpa Sistem Escrow (Rekening Bersama):** Platform tidak memproses aliran uang transaksi di dalam sistem. Tidak ada pemotongan MDR (Merchant Discount Rate) dan tidak ada penahanan dana pedagang. Arus kas langsung masuk ke rekening pribadi atau tunai pedagang saat transaksi.
3. **Tanpa Registrasi Akun dan Dasbor Rumit:** Penjual tidak dibebani proses pembuatan akun berbelit (username, password, verifikasi email berlapis) maupun dasbor manajemen inventaris berbasis desktop. Penjual cukup menggunakan formulir web ringkas dari peramban ponsel.
4. **Fokus Hyperlocal Radius Mikro (<3–5 KM):** Platform memprioritaskan penemuan berbasis radius fisik terdekat untuk memastikan interaksi jual-beli berlangsung relevan antar-warga satu lingkungan.
5. **Transaksi Dialihkan ke WhatsApp (Discovery Tool, Bukan Checkout Engine):** Fungsi platform dibatasi sebagai jembatan penemuan (discovery tool). Konfirmasi ketersediaan barang, kesepakatan harga, varian, dan pembayaran diselesaikan secara personal melalui chat WhatsApp via tombol direct 1-click.
6. **Peniadaan Biaya Kurir Pihak Ketiga (Fokus Pemenuhan Mandiri):** Seluruh produk wajib memiliki kejelasan metode pemenuhan mandiri, yaitu diambil sendiri oleh pembeli (Self-Pickup) atau diantar langsung oleh pedagang (Antar Mandiri), guna mengeliminasi komponen ongkir kurir instan yang mahal.
7. **Kemudahan Akses Peramban Bergerak (Mobile-First Web):** Antarmuka dirancang optimal untuk peramban ponsel pintar tanpa mewajibkan pembeli maupun penjual mengunduh aplikasi berukuran besar.

---

## 4. Lingkup Fitur MVP (5 Fitur MUST HAVE)

Mengacu persis pada kuadran MUST HAVE tabel MoSCoW dokumen 05-mvp.md (Bagian 5), lingkup rilis perdana mencakup 5 fitur utama berikut:

### 4.1. Deteksi Lokasi & Filter Radius Mikro (<3–5 KM)
* **Deskripsi:** Sistem mendeteksi lokasi pembeli melalui koordinat peramban (GPS) atau input wilayah manual, kemudian menyaring katalog produk yang berada dalam radius terdekat (<3–5 KM) dan mengurutkannya berdasarkan jarak fisik paling dekat.
* **User Story:**
  * Sebagai calon pembeli lokal,
  * saya ingin sistem mendeteksi lokasi saya atau memilih kelurahan terdekat dan menampilkan produk dalam radius <3–5 KM,
  * agar saya hanya melihat produk jualan tetangga di lingkungan sekitar yang bebas dari kendala ongkos kirim mahal.
* **Acceptance Criteria:**
  * Sistem memunculkan permintaan izin akses lokasi peramban (Geolocation API) saat pembeli pertama kali membuka halaman.
  * Jika izin lokasi disetujui, sistem menghitung jarak fisik antara pembeli dan penjual, lalu memfilter produk yang berada dalam radius <3–5 KM.
  * Daftar produk yang lolos filter ditampilkan berurutan dari jarak yang paling dekat ke jarak yang lebih jauh (misal: "0.4 KM dari Anda").
  * Jika izin lokasi ditolak atau tidak didukung perangkat, sistem menyediakan pilihan pemilihan wilayah/kelurahan secara manual (usulan) tanpa menampilkan galat layar kosong.
  * Produk di luar batas radius maksimal (<3–5 KM) tidak ditampilkan pada etalase utama.

### 4.2. Katalog Produk Sederhana (Foto, Nama, Harga, Deskripsi Singkat)
* **Deskripsi:** Halaman etalase publik dan kartu tampilan produk yang memuat informasi pokok: foto produk, nama produk/makanan, nominal harga (IDR), deskripsi singkat, nama toko/penjual, serta indikator jarak dari pembeli.
* **User Story:**
  * Sebagai calon pembeli,
  * saya ingin melihat kartu katalog produk dengan foto yang jelas, nama, harga, dan deskripsi ringkas,
  * agar saya memperoleh informasi dasar yang memadai untuk menentukan keputusan pembelian secara cepat.
* **Acceptance Criteria:**
  * Katalog menampilkan daftar kartu produk yang responsif pada layar ponsel pintar.
  * Setiap kartu produk wajib memuat: foto produk, nama produk, harga dalam format mata uang Rupiah (contoh: Rp25.000), nama usaha/penjual, dan perkiraan jarak fisik.
  * Kartu produk dapat diketuk untuk membuka rincian yang menyertakan deskripsi singkat produk dan label metode pemenuhan.
  * Tampilan gambar dimuat secara optimal tanpa distorsi aspek rasio dan hemat kuota data seluler.

### 4.3. Tombol Direct-to-WhatsApp (1-Click) dengan Template Pesan Otomatis
* **Deskripsi:** Tombol panggilan aksi utama (Call to Action) pada rincian produk yang ketika diketuk langsung mengarahkan pembeli ke aplikasi WhatsApp penjual dengan draf pesan pesanan yang telah terisi otomatis.
* **User Story:**
  * Sebagai pembeli,
  * saya ingin menekan tombol WhatsApp yang otomatis menyiapkan teks pesanan berisi rincian produk,
  * agar saya dapat langsung memesan ke penjual tanpa perlu menyimpan nomor kontak atau mengetik ulang rincian pesanan secara manual.
* **Acceptance Criteria:**
  * Tombol aksi "Pesan via WhatsApp" tersedia secara jelas pada setiap rincian produk.
  * Mengetuk tombol akan memicu pemanggilan URL protokol `https://wa.me/<nomor_penjual>?text=<pesan_terformat>`.
  * Nomor telepon penjual secara otomatis diformat ke standar internasional tanpa awalan nol, tanda tambah, atau karakter pemisah (contoh: 08123456789 menjadi 628123456789).
  * Teks pesan otomatis mencantumkan sekurang-kurangnya: nama produk, jumlah default (1), metode pengambilan yang dipilih, dan sapaan pembuka.
  * Aksi berhasil membuka aplikasi WhatsApp pada perangkat ponsel pembeli atau WhatsApp Web pada peramban desktop.

### 4.4. Formulir Unggah Cepat via HP (Tanpa Dasbor Rumit)
* **Deskripsi:** Halaman formulir web sederhana berbasis peramban ponsel bagi penjual untuk menayangkan produk dengan memasukkan data pokok tanpa melalui registrasi akun, pembuatan kata sandi, atau pengelolaan dasbor toko komputer.
* **User Story:**
  * Sebagai penjual rumahan,
  * saya ingin mengunggah foto dan rincian produk jualan melalui formulir singkat di peramban ponsel,
  * agar produk saya dapat langsung tayang di katalog lokal tanpa hambatan teknis pendaftaran akun yang rumit.
* **Acceptance Criteria:**
  * Formulir dapat diakses langsung tanpa proses login, registrasi akun pengguna, atau verifikasi email/nomor telepon yang memblokir alur.
  * Formulir memuat field input wajib: Nama Usaha, Foto Produk, Nama Produk, Harga (angka), Nomor WhatsApp aktif, Titik Lokasi/Kelurahan Penjual (usulan), dan Opsi Pemenuhan.
  * Formulir menyediakan fitur pengambilan foto langsung dari kamera ponsel atau galeri gambar.
  * Sistem melakukan validasi input mendasar di sisi klien: nomor WhatsApp valid, harga bernilai angka positif, serta foto dan nama produk tidak boleh kosong.
  * Setelah tombol publikasi ditekan, data produk tersimpan dan langsung muncul pada katalog pencarian radius pembeli.

### 4.5. Label Opsi Ambil Sendiri / Antar Lokal (Penanda Opsi Pengambilan)
* **Deskripsi:** Penanda visual yang tegas pada setiap kartu produk yang menunjukkan metode pemenuhan pesanan yang disediakan penjual: apakah pembeli dapat mengambil sendiri ke lokasi penjual (Self-Pickup) atau dapat diantar langsung oleh penjual (Antar Mandiri).
* **User Story:**
  * Sebagai pembeli,
  * saya ingin melihat label opsi pengambilan mandiri atau antar langsung pada produk yang saya minati,
  * agar saya mengetahui sejak awal bagaimana pesanan akan saya terima tanpa biaya kurir pihak ketiga.
* **Acceptance Criteria:**
  * Pada formulir unggah, penjual wajib mencentang sekurang-kurangnya satu opsi pemenuhan: "Bisa Ambil di Tempat" atau "Bisa Diantar Penjual" (bisa memilih keduanya).
  * Setiap kartu produk di etalase dan halaman rincian produk memuat lencana/label visual status pemenuhan sesuai pilihan penjual.
  * Pilihan opsi pemenuhan yang dipilih pembeli disematkan ke dalam draf template teks pesan WhatsApp saat tombol pemesanan diketuk.

---

## 5. User Flow Penjual dan Pembeli

Mengacu pada bagian 6 dokumen 05-mvp.md, berikut adalah alur pengguna bernomor untuk kedua belah pihak:

### 5.1. Alur Pengguna Penjual (Seller Flow)
1. Penjual membuka platform web Dekat.in melalui peramban pada ponsel pintar.
2. Penjual menekan tombol "Tambah Jualan" atau "Jual Produk" pada halaman utama.
3. Penjual mengisi formulir singkat unggah produk yang memuat:
   * Nama usaha / toko rumahan
   * Foto produk (unggah dari galeri atau kamera ponsel)
   * Nama produk
   * Harga jual (dalam Rupiah)
   * Deskripsi singkat produk
   * Nomor WhatsApp aktif
   * Penentuan lokasi usaha/penjual (menggunakan deteksi GPS lokasi saat ini atau memilih kelurahan/kecamatan) (usulan)
   * Pilihan metode pemenuhan pesanan (Bisa Ambil di Tempat / Bisa Diantar Penjual / Keduanya)
4. Penjual menekan tombol "Tayangkan Produk".
5. Produk langsung terbit dan tayang di katalog lokal tanpa melalui proses verifikasi rumit.
6. Penjual menerima notifikasi pemesanan langsung dari calon pembeli berupa pesan obrolan di aplikasi WhatsApp dengan format rincian pesanan yang sudah terisi otomatis.
7. Penjual membalas chat pembeli untuk mengonfirmasi ketersediaan stok, menyepakati waktu pengambilan/pengantaran, serta memberikan nomor rekening atau QRIS statis untuk pembayaran.

### 5.2. Alur Pengguna Pembeli (Buyer Flow)
1. Pembeli membuka platform web Dekat.in melalui peramban pada perangkat ponsel atau komputer.
2. Pembeli menerima dialog permohonan izin akses lokasi peramban (GPS) dan memberikan persetujuan izin (atau memilih area kelurahan/kecamatan secara manual bila GPS tidak aktif).
3. Pembeli melihat etalase produk makanan dan produk rumahan di sekitarnya dalam radius <3–5 KM yang secara otomatis diurutkan dari jarak paling dekat.
4. Pembeli menelusuri etalase dan memilih kartu produk yang diminati untuk melihat rincian informasi.
5. Pembeli memeriksa detail produk, foto, harga, deskripsi singkat, dan penanda metode pengambilan (Self-Pickup atau Antar Mandiri).
6. Pembeli menentukan pilihan metode pemenuhan yang diinginkan (ambil sendiri atau diantar).
7. Pembeli menekan tombol "Pesan via WhatsApp".
8. Peramban secara otomatis membuka aplikasi WhatsApp menuju kontak penjual dengan teks draf pemesanan yang telah terformat lengkap.
9. Pembeli mengirimkan pesan tersebut dan melanjutkan kesepakatan transaksi, pembayaran (transfer langsung/QRIS/tunai), serta penerimaan barang langsung dengan penjual tanpa perantara.

---

## 6. Usulan Antarmuka, Struktur Data Minimal, dan Integrasi WhatsApp

### 6.1. Usulan Daftar Layar / Halaman MVP
1. **Layar 1 — Beranda / Etalase Hyperlocal (Buyer Catalog):**
   * Header: Logo Dekat.in, indikator lokasi pengguna saat ini (misal: "Sekitar Depok, Sleman"), dan tombol "Ubah Lokasi".
   * Bilah Filter Jarak: Penanda radius aktif (<3 KM atau <5 KM).
   * Konten Utama: Daftar kartu produk terdekat (grid/list) yang menampilkan foto, nama produk, harga, nama penjual, jarak (KM), dan badge pemenuhan (Ambil Sendiri / Antar Mandiri).
   * Tombol Aksi Melayang (Floating Action Button): Tombol pintas "Jual Produk" untuk penjual.
2. **Layar 2 — Pemilihan Lokasi Manual (Modal/Popup):**
   * Muncul jika akses GPS ditolak atau jika pembeli ingin mengganti titik pantau.
   * Input pencarian atau pilihan dropdown kecamatan dan kelurahan fokus (Depok, Mlati, Ngaglik).
3. **Layar 3 — Modal / Rincian Produk (Product Detail):**
   * Tampilan foto produk ukuran penuh.
   * Judul produk, nominal harga, nama penjual, dan estimasi jarak fisik.
   * Teks deskripsi singkat produk.
   * Penanda metode pemenuhan pesanan (opsi radio/tombol untuk memilih: "Ambil Sendiri" atau "Diantar Penjual").
   * Tombol Call to Action utama: "Pesan via WhatsApp".
4. **Layar 4 — Formulir Unggah Cepat Penjual (Quick Mobile Form):**
   * Tampilan satu kolom yang ramah peramban ponsel.
   * Area unggah gambar (preview foto).
   * Form isian: Nama Usaha, Nama Produk, Harga (Rp), Deskripsi Singkat, Nomor WhatsApp, Penentuan Lokasi (tombol "Ambil Koordinat Saya" dan dropdown Kelurahan), serta Kotak Centang Opsi Pemenuhan.
   * Tombol utama: "Tayangkan Produk Sekarang".
5. **Layar 5 — Konfirmasi Sukses Tayang (Publish Success):**
   * Halaman status ringkas yang memberitahukan produk berhasil tayang.
   * Tombol untuk melihat langsung tampilan produk di katalog dan tombol tautan bagikan (share link) ke media sosial/status WhatsApp penjual (usulan).

### 6.2. Field Data Minimal

#### Entitas Penjual (Seller)
| Nama Field | Tipe Data | Sifat | Keterangan |
| :--- | :--- | :--- | :--- |
| `seller_name` | String | Wajib | Nama usaha atau nama penjual rumahan (contoh: "Dimsum Bu Ratna"). |
| `whatsapp_number` | String | Wajib | Nomor WhatsApp aktif penjual dalam format angka (contoh: "081234567890"). |
| `seller_lat` (usulan) | Float/Decimal | Wajib | Koordinat latitude penjual untuk kalkulasi radius jarak terhadap pembeli. |
| `seller_lng` (usulan) | Float/Decimal | Wajib | Koordinat longitude penjual untuk kalkulasi radius jarak terhadap pembeli. |
| `subdistrict` (usulan) | String | Wajib | Nama kelurahan/desa domisili penjual sebagai cadangan filter. |
| `district` (usulan) | String | Wajib | Nama kecamatan domisili penjual (Depok, Mlati, atau Ngaglik). |
| `pickup_available` | Boolean | Wajib | Penanda apakah pesanan dapat diambil sendiri oleh pembeli (Self-Pickup). |
| `delivery_available` | Boolean | Wajib | Penanda apakah penjual melayani pengantaran mandiri langsung (Antar Lokal). |

#### Entitas Produk (Product)
| Nama Field | Tipe Data | Sifat | Keterangan |
| :--- | :--- | :--- | :--- |
| `product_id` (usulan) | String/UUID | Wajib (Sistem) | Pengenal unik produk dalam sistem basis data. |
| `seller_id` (usulan) | String/UUID | Wajib (Sistem) | Relasi produk terhadap entitas penjual. |
| `product_name` | String | Wajib | Nama produk atau makanan yang dijual (contoh: "Dimsum Ayam Homemade"). |
| `price` | Integer | Wajib | Harga jual produk dalam satuan mata uang Rupiah (contoh: 30000). |
| `image_url` | String | Wajib | Tautan berkas foto produk hasil pengunggahan. |
| `description` | String | Wajib | Penjelasan singkat produk, porsi, atau ketentuan pesanan. |
| `variant_options` (usulan) | String | Opsional | Pilihan rasa, varian, atau ukuran jika tersedia (contoh: "Original, Pedas"). |
| `created_at` (usulan) | Timestamp | Wajib (Sistem) | Waktu pengunggahan produk untuk keperluan masa tayang dan pengurutan. |

### 6.3. Format Integrasi dan Template Pesan WhatsApp

#### Template Pesan Otomatis (Format Teks Dasar)
```text
Halo [Nama Usaha], saya melihat produk [Nama Produk] di Dekat.in.
Saya ingin memesan:
- Produk: [Nama Produk]
- Varian: [Varian Produk / -]
- Jumlah: [Jumlah Pesanan]
- Metode Pengambilan: [Ambil Sendiri di Tempat (Self-Pickup) / Diantar Penjual (Antar Mandiri)]
- Catatan Tambahan: [Catatan / Alamat Pembeli]

Apakah pesanan ini masih tersedia? Terima kasih!
```

#### Contoh Konkret Template Pesan
```text
Halo Dimsum Bu Ratna, saya melihat produk Dimsum Ayam Homemade di Dekat.in.
Saya ingin memesan:
- Produk: Dimsum Ayam Homemade
- Varian: Pedas Manis
- Jumlah: 2 porsi
- Metode Pengambilan: Ambil Sendiri di Tempat (Self-Pickup)
- Catatan Tambahan: Diambil sekitar pukul 16.30 WIB sore ini

Apakah pesanan ini masih tersedia? Terima kasih!
```

#### Format URL Standar `wa.me`
Tautan dibentuk menggunakan pola:
`https://wa.me/<nomor_telepon_internasional>?text=<url_encoded_pesan>`

Ketentuan nomor: Angka `0` di awal nomor lokal wajib diganti kode negara `62` tanpa tanda `+`, spasi, atau tanda minus. Contoh nomor `081234567890` dikonversi menjadi `6281234567890`.

#### Contoh URL Lengkap yang Dihasilkan
```text
https://wa.me/6281234567890?text=Halo%20Dimsum%20Bu%20Ratna%2C%20saya%20melihat%20produk%20Dimsum%20Ayam%20Homemade%20di%20Dekat.in.%0ASaya%20ingin%20memesan%3A%0A-%20Produk%3A%20Dimsum%20Ayam%20Homemade%0A-%20Varian%3A%20Pedas%20Manis%0A-%20Jumlah%3A%202%20porsi%0A-%20Metode%20Pengambilan%3A%20Ambil%20Sendiri%20di%20Tempat%20%28Self-Pickup%29%0A-%20Catatan%20Tambahan%3A%20Diambil%20sekitar%20pukul%2016.30%20WIB%20sore%20ini%0A%0AApakah%20pesanan%20ini%20masih%20tersedia%3F%20Terima%20kasih%21
```

---

## 7. Di Luar Lingkup (Out of Scope) & Roadmap Pengembangan

Mengacu pada kuadran MoSCoW dan rencana pengembangan bertahap pada dokumen 05-mvp.md (Bagian 5 dan 7), batasan fitur non-MVP dibagi menjadi:

### 7.1. SHOULD HAVE (Fase 2: Validasi Komunitas & Kenyamanan)
Fitur yang memiliki nilai tambah signifikan namun tidak menggagalkan peluncuran perdana jika ditiadakan pada MVP:
1. **Kolom Pencarian Kata Kunci (Search Bar) & Filter Kategori:** Fasilitas bagi pembeli untuk mencari nama makanan tertentu atau memfilter kategori (Makanan, Minuman, Kerajinan, Makanan Halal/Vegetarian).
2. **Tautan Titik Penjemputan ke Google Maps:** Integrasi tautan statis untuk membuka rute Google Maps menuju alamat penjual saat pembeli memilih opsi Self-Pickup. *(Catatan: Pada dokumen 05 terdapat duplikasi butir 2 dan butir 3 yang merujuk pada integrasi peta penjemputan yang sama).*
3. **Indikator Status Toko (Buka / Tutup):** Penanda visual apakah penjual sedang aktif menerima pesanan hari ini atau sedang tutup.

### 7.2. COULD HAVE (Fase 3 & Fase 4)
Fitur yang hanya dikembangkan jika hipotesis adopsi lokal telah tervalidasi dan sistem berada pada tahap pertumbuhan:
1. **Sistem Ulasan & Testimoni Warung (Fase 3: Kepercayaan & Reputasi):** Fasilitas bagi pembeli untuk memberikan rating bintang 1–5 dan ulasan komentar berbasis komunitas sekitar.
2. **Lencana Profil Penjual Terverifikasi (Fase 3: Kepercayaan & Reputasi):** Badge verifikasi warga lokal melalui kerja sama pengurus RT/RW, Dukuh, atau asosiasi paguyuban kos.
3. **Fitur Promosi Berbayar Ringan / Featured Listing (Fase 4: Monetisasi & Skalabilitas):** Penyematan produk di baris paling atas etalase radius dengan biaya iklan terjangkau (contoh: Rp10.000/minggu).
4. **Tampilan Peta Interaktif (Interactive Map Pinpoint) (Fase 4: Skalabilitas):** Antarmuka peta digital yang dapat digeser dan diperbesar untuk melihat sebaran titik jualan secara spasial.

### 7.3. WON'T HAVE (Dieliminasi dari Rilis Perdana)
Fitur yang secara sadar diputuskan TIDAK dibuat karena bertentangan dengan proposisi nilai dasar atau menimbulkan kompleksitas berlebih:
1. **In-App Payment Gateway & Sistem Escrow (Rekening Bersama):** Dieliminasi karena mengenakan potongan komisi/MDR yang melanggar janji 0% komisi, menahan uang tunai harian pedagang, dan membutuhkan kepatuhan regulasi finansial yang rumit.
2. **Pelacakan Kurir Real-Time (Live GPS Courier Tracking):** Dieliminasi karena tidak relevan dengan model pemenuhan mandiri (ambil sendiri atau diantar pedagang) serta memboroskan kuota internet dan beban komputasi server.
3. **Keranjang Belanja Multi-Penjual (Multi-Merchant Cart):** Dieliminasi karena alur transaksi diarahkan langsung ke masing-masing obrolan WhatsApp penjual independen.

---

## 8. Metrik Keberhasilan Awal

Target metrik keberhasilan awal diturunkan langsung dari kalkulasi Serviceable Obtainable Market (SOM) pada dokumen 04-vpc-bmc.md (Bagian 3), dilengkapi dengan usulan indikator operasional produk:

### 8.1. Metrik Target Berdasarkan Dokumen Sumber (04-vpc-bmc.md — SOM Tahun Pertama)
* **Jumlah Penjual Terdaftar:** Mencapai **500 – 1.000 penjual rumahan** di tahun pertama peluncuran.
* **Jumlah Pengguna Pembeli Aktif:** Mencapai **15.000 pengguna aktif pembeli lokal** di tahun pertama peluncuran.
* **Wilayah Target Operasional Awal:** Berfokus pada **3 kecamatan** padat mahasiswa, kos-kosan, dan pemukiman di Kabupaten Sleman, Daerah Istimewa Yogyakarta, yaitu:
  1. Kecamatan Depok
  2. Kecamatan Mlati
  3. Kecamatan Ngaglik

### 8.2. Metrik Operasional & Kualitas Produk MVP (usulan)
Untuk memantau kesehatan produk pada fase rilis awal, ditetapkan metrik operasional berikut:
1. **Rasio Klik Tombol WhatsApp (WhatsApp Click-Through Rate) (usulan):** Minimal 10%–15% dari total kunjungan rincian produk berlanjut pada penekanan tombol "Pesan via WhatsApp".
2. **Tingkat Keberhasilan Pengunggahan Produk (Form Completion Rate) (usulan):** Lebih dari 85% penjual yang membuka halaman formulir berhasil menuntaskan pengunggahan produk hingga tayang.
3. **Waktu Unggah Produk (Time to Publish) (usulan):** Rata-rata waktu pengisian formulir hingga produk terbit di bawah 2 menit pada peramban ponsel.
4. **Kerapatan Katalog Lokal (Local Listing Density) (usulan):** Minimal 15–20 produk aktif per radius 3 KM di setiap kelurahan fokus untuk mencegah pembeli melihat katalog kosong (*cold start problem*).
5. **Rasio Kunjungan Berulang Pembeli (Repeat Buyer Ratio) (usulan):** Minimal 20% pembeli kembali membuka etalase Dekat.in dalam periode 14 hari.

---

## 9. Pertanyaan Terbuka & Inkonsistensi Dokumen Sumber

Berdasarkan penelaahan komprehensif terhadap dokumen 02, 03, 04, dan 05, ditemukan sejumlah kontradiksi, celah logika, dan inkonsistensi yang perlu diselesaikan oleh tim:

1. **Kesalahan Penomoran Kelompok (03 vs 02/04/05):**
   * Pada dokumen `03-customer-discovery.md` Bagian 11 (Kesimpulan), tertulis kalimat: *"secara fundamental mengubah arah strategi kelompok 12"*.
   * Padahal pada header dokumen 02, 03, 04, 05 dan kesimpulan dokumen 04, kelompok yang bersangkutan secara konsisten adalah **Kelompok 11**.

2. **Inkonsistensi Batasan Radius Hyperlocal:**
   * Di `02-creative-thinking.md` Solusi A1, cakupan wilayah masih menggunakan skala luas "per kota/kecamatan".
   * Di `03-customer-discovery.md`, Bagian 8 & 11 menyebut "<5 km" dan Responden 1 menyebut "maksimal 5KM", namun di Bagian 9 menyebut "radius terdekat (misal <3KM)", dan Responden 5 menyebut "radius 2 km".
   * Di `04-vpc-bmc.md`, Bagian 1.1 menyebut "<3-5 KM", Value Proposition Statement menyebut tegas "radius 5 KM", dan BMC Blok 2 menyebut "<5 KM".
   * Di `05-mvp.md`, judul fitur dan MoSCoW menuliskan "<3–5 KM".
   * *Masalah Terbuka:* Belum ada ketetapan angka pasti apakah batas radius default sistem adalah 3 KM atau 5 KM, atau apakah pengguna diberikan kontrol filter geser (misal: pilihan 1 KM, 3 KM, 5 KM) (usulan).

3. **Duplikasi Butir Fitur pada Kategori SHOULD HAVE (05-mvp.md):**
   * Pada tabel MoSCoW kuadran SHOULD HAVE dokumen 05-mvp.md, tercantum dua butir yang identik:
     * Butir 2: *"Tautan Titik Penjemputan ke Google Maps"*
     * Butir 3: *"Tautan statis buka maps"*
   * Kedua butir ini jelas merupakan duplikasi penulisan untuk fungsi yang sama.

4. **Kontradiksi Konsep "Terverifikasi/Terkurasi" vs "Tanpa Verifikasi Rumit":**
   * Di dokumen `04-vpc-bmc.md` blok *Key Resources* dan *Key Activities*, tertulis: *"Basis data profil pedagang dan katalog produk lokal yang terverifikasi"* serta *"Kurasi, verifikasi keaslian, dan pembaruan data produk UMKM lokal"*.
   * Sebaliknya, di dokumen `05-mvp.md` (Alur Penjual) dan dokumen 04 (*Value Map*), ditekankan bahwa produk *"langsung tayang di katalog lokal tanpa verifikasi rumit"* dan *"tanpa sistem registrasi rumit"*.
   * *Masalah Terbuka:* Mekanisme "langsung tayang tanpa verifikasi" sangat rentan disalahgunakan untuk spam, nomor WhatsApp fiktif, produk ilegal/tidak pantas, atau penipuan harga. Belum ada mekanisme kurasi moderasi pasca-tayang yang dirumuskan untuk mengatasi risiko ini.

5. **Ketiadaan Mekanisme Manajemen Produk Penjual (Edit & Hapus Produk):**
   * MVP menetapkan prinsip "tanpa pembuatan akun dan tanpa dasbor".
   * *Masalah Terbuka:* Jika penjual tidak memiliki akun atau sesi login, bagaimana cara penjual mengubah harga, memperbarui foto, menandai produk sedang habis, atau menghapus produk yang sudah tidak dijual? Jika harus mengunggah ulang, hal ini akan memicu duplikasi data produk usang di etalase pembeli.

6. **Ketiadaan Input Lokasi Penjual pada Alur Formulir Unggah MVP:**
   * Fitur 1 (Pendeteksi Lokasi & Filter Radius) menuntut penghitungan jarak fisik matematis antara pembeli dan penjual (<3–5 KM).
   * Namun pada dokumen `05-mvp.md` Bagian 6 (Alur Pengguna Sisi Penjual), field yang wajib diisi penjual hanya tercatat: *"nama usaha, foto produk, nama produk, harga, nomor WhatsApp, dan pilihan metode pemenuhan"*. Tidak ada field untuk memasukkan alamat, koordinat GPS, atau kelurahan penjual.
   * Tanpa data titik lokasi penjual, sistem tidak akan pernah bisa menghitung jarak atau memfilter radius produk bagi pembeli. Field koordinat/kelurahan penjual mutlak harus ditambahkan ke formulir (usulan).

7. **Ketiadaan Input Deskripsi Produk pada Alur Pengguna Penjual:**
   * Pada dokumen `05-mvp.md` Fitur 2 (Katalog Produk Sederhana), deskripsi fitur mencakup *"Foto, Nama, Harga, Deskripsi Singkat"*.
   * Namun pada Alur Pengguna Penjual (Bagian 6 di 05-mvp.md), butir "deskripsi singkat" tidak dicantumkan dalam daftar isian formulir penjual.

8. **Inkonsistensi Logika pada Tabel Litmus Test (05-mvp.md):**
   * Pada tabel evaluasi Litmus Test (baris 54) untuk Fitur 5 (*Penanda Opsi Self-Pickup / Antar Mandiri*), pertanyaan uji *"Tanpa fitur ini, apakah masalah utama pengguna masih selesai?"* dijawab dengan nilai **"MASIH BISA"**.
   * Berdasarkan kaidah Litmus Test, fitur yang dijawab "MASIH BISA" secara metodologis diklasifikasikan sebagai fitur tambahan yang dapat ditunda (non-MVP, sebagaimana fitur 6–10). Namun pada kolom keputusan, fitur ini tetap dipaksakan berstatus **"FITUR INTI (MVP)"**.

9. **Anomali Penggabungan Responden Wawancara pada Dokumen 03:**
   * Pada tabel ringkasan wawancara dokumen `03-customer-discovery.md` baris 36, data Responden 9 (Bu Sri, 52 tahun) dan Responden 10 (Arif, 24 tahun) tergabung dalam satu baris sel tabel markdown tanpa pemisah baris tabel yang benar, sehingga data profil dan kutipan Arif terselip di ujung teks Bu Sri.

10. **Tantangan Operasional Fitur Promosi Berbayar (Featured Listing) Tanpa Akun:**
    * Di dokumen `04-vpc-bmc.md` (Revenue Streams) dan `05-mvp.md` (Roadmap Fase 4), terdapat rencana monetisasi *Featured Listing* seharga Rp10.000/minggu.
    * Karena platform tidak memiliki akun penjual dan tidak memiliki payment gateway terintegrasi, proses pembayaran, verifikasi transfer manual, serta aktivasi status promosi berbayar berpotensi menimbulkan beban operasional manual yang sangat tinggi bagi pengelola.

11. **Ketiadaan Visibilitas Konversi Transaksi Nyata:**
    * Karena platform hanya bertindak sebagai discovery tool dan mengalihkan pembeli ke WhatsApp, Dekat.in tidak memiliki data pencatatan apakah pesanan yang dikirimkan via WhatsApp berakhir dengan transaksi jual-beli nyata, dibatalkan, atau tidak direspons oleh penjual. Metrik yang dapat dipantau sistem murni sebatas klik tombol pesan (*click-through rate*).
