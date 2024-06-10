body { font-family: 'Times New Roman', Times, serif, sans-serif; /* Ganti font default */ margin: 0; padding: 0; }

header, footer { background-color: #1e33a8; /* Warna latar belakang header / padding: 1rem; / Padding untuk memberikan ruang di sekitar elemen header */ text-align: center; }

.penutupan , .Judul{ background-color: #54f0d6; padding : 1rem; text-align: center; width: 500px; height: 40px; border-radius: 10px; backdrop-filter: blur(10px); box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); margin: 1rem auto; }

.penutupan, .Judul { padding-bottom: 40px; }

main { display: flex; /* Menggunakan flexbox untuk menata card secara horizontal / flex-wrap: wrap; / Memungkinkan card untuk pindah ke baris berikutnya saat lebar layar terlalu kecil / justify-content: center; / Pusatkan card secara horizontal / padding: 1rem; / Padding untuk memberikan ruang di sekitar elemen main */ height: 450px; }

.input { border: none; padding: 1rem; border-radius: 1rem; background: #e8e8e8; box-shadow: 20px 20px 60px #c5c5c5, -20px -20px 60px #ffffff; transition: 0.3s; width: 300px; /* Sesuaikan lebar input dengan kebutuhan */ }

.input:focus { outline-color: #e8e8e8; background: #e8e8e8; box-shadow: inset 20px 20px 60px #c5c5c5, inset -20px -20px 60px #ffffff; transition: 0.3s; }

.card { position: relative; width: 220px; height: 320px; background: #54f0d6(128, 196, 255); display: flex; align-items: center; justify-content: center; font-size: 25px; font-weight: bold; border-radius: 15px; cursor: pointer; margin: 1rem; /* Tambahkan margin agar card tidak rapat satu sama lain */ }

.card::before, .card::after { position: absolute; content: ""; width: 20%; height: 20%; display: flex; align-items: center; justify-content: center; font-size: 15px; font-weight: bold; background-color: rgb(160, 231, 255); transition: all 0.5s; }

.card::before { top: 0; right: 0; border-radius: 0 15px 0 100%; }

.card::after { bottom: 0; left: 0; border-radius: 0 100% 0 15px; }

.card:hover::before, .card:hover:after { width: 100%; height: 100%; border-radius: 15px; transition: all 0.3s; }

.card[id="card1"]:hover::after { content: "Aplikasi memiliki fitur untuk merekam semua aktivitas yang terkait dengan implementasi perangkat lunak, seperti pengembangan, pengujian, dan penyebaran."; }

.card[id="card2"]:hover::after { content: "Aplikasi dapat merekam data transaksi model, yang mencakup input fitur yang digunakan untuk melatih model, serta label output yang dihasilkan oleh model."; }

.card[id="card3"]:hover::after { content: "Aplikasi mengumpulkan dan menyimpan data tentang lingkungan yang relevan dengan implementasi perangkat lunak, seperti sistem operasi, versi perangkat lunak, perangkat keras yang digunakan, dll."; }

.card[id="card4"]:hover::after { content: "Aplikasi memungkinkan pemelihara perangkat lunak untuk memberikan masukan dan catatan terkait dengan implementasi dan pemeliharaan perangkat lunak."; }

.card[id="card5"]:hover::after { content: "Aplikasi dilengkapi dengan fitur pemantauan kinerja untuk memantau performa perangkat lunak yang sudah terpasang di lingkungan produksi."; }

Penjelasan: Kode CSS di atas digunakan untuk mengatur tata letak dan gaya visual dari sebuah halaman web atau aplikasi berbasis web. Berikut penjelasan singkat tentang setiap bagian kode:

Body Styling:

Mengatur font default menjadi Times New Roman, dengan backup font berupa Times, serif, dan sans-serif.
Margin dan padding diatur menjadi 0 untuk menghilangkan ruang tambahan di sekitar elemen body.
Header dan Footer Styling:

Background-color ditetapkan menjadi biru (#1e33a8) untuk header dan footer.
Padding 1rem digunakan untuk memberikan ruang di sekitar elemen header dan footer.
Teks ditengahkan menggunakan text-align: center;.
Styling untuk Kelas .penutupan dan .Judul:

Kedua kelas ini memiliki background-color yang berbeda (#54f0d6).
Padding 1rem digunakan untuk memberikan ruang di sekitar elemen.
Text ditengahkan menggunakan text-align: center;.
Width ditetapkan menjadi 500px untuk membatasi lebar elemen.
Tinggi elemen ditetapkan menjadi 40px.
Border-radius digunakan untuk membuat sudut elemen melengkung.
Backdrop-filter: blur(10px) digunakan untuk memberikan efek blur pada latar belakang dengan ketebalan 10px.
Box-shadow ditambahkan untuk memberikan efek bayangan yang lembut.
Terdapat duplikasi pengaturan padding-bottom yang seharusnya hanya ada di .penutupan.
Styling untuk Bagian Main:

Display flex digunakan untuk menata card secara horizontal.
Flex-wrap diatur menjadi wrap untuk memungkinkan card untuk pindah ke baris berikutnya saat lebar layar terlalu kecil.
Justify-content diatur menjadi center untuk memusatkan card secara horizontal.
Padding 1rem digunakan untuk memberikan ruang di sekitar elemen main.
Tinggi elemen ditetapkan menjadi 450px.
Styling untuk Input:

Input diberi border-none untuk menghilangkan border bawaan.
Padding ditetapkan menjadi 1rem untuk memberikan ruang di dalam input.
Border-radius digunakan untuk membuat sudut elemen melengkung.
Background color dan box-shadow digunakan untuk memberikan efek visual pada input.
Transition 0.3s digunakan untuk memberikan efek transisi halus saat input difokuskan.
Styling untuk Card:

Position diatur menjadi relative untuk memungkinkan penempatan absolut pada pseudo-elemen.
Lebar dan tinggi ditetapkan untuk card.
Background-color digunakan untuk memberikan warna latar belakang pada card.
Display flex dan align-items center serta justify-content center digunakan untuk memusatkan teks di dalam card.
Font-size dan font-weight ditetapkan untuk teks di dalam card.
Border-radius digunakan untuk membuat sudut card melengkung.
Cursor dinyatakan sebagai pointer untuk menunjukkan bahwa card dapat di-klik.
Terdapat pseudo-elemen (::before dan ::after) yang digunakan untuk menampilkan informasi tambahan saat card di-hover.
Pseudo-elemen ::before dan ::after memiliki transition untuk memberikan efek transisi saat di-hover.
Pseudo-elemen Hover untuk Setiap Card:

Saat card di-hover, konten dari pseudo-elemen ::after akan ditampilkan sesuai dengan konten yang
