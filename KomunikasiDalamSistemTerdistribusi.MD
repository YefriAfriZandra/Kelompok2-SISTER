# Komunikasi dalam Sistem Terdistribusi

**Nama : Libryan Adetya Syafithree**

**NIM  : 2111081008**

## I. Protokol komunikasi

Protokol adalah sebuah aturan atau standar yang mengatur atau mengijinkan terjadinya hubungan, komunikasi, dan perpindahan data antara dua atau lebih titik komputer. Protokol dapat diterapkan pada perangkat keras, perangkat lunak atau kombinasi dari keduanya. Pada waktu itu, komunikasi antar komputer dari vendor yang berbeda adalah sangat sulit dilakukan, karena mengunakan protokol dan format data yang berbeda-beda. Sehingga International Standards Organization (ISO) membuat suatu arsitektur komunikasi yang dikenal sebagai Open System Interconnection (OSI) model yang mendefinisikan standar untuk menghubungkan komputer-komputer dari vendor-vendor yang berbeda. Model-OSI tersebut terbagi atas layer-layer, yaitu:

  1. Physical Layer
  2. Data Link
  3. Network
  4. Transport
  5. Session
  6. Presentation
  7. Application.

### Komunikasi memiliki komponen-komponen yang menjadikan komunikasi berjalan dengan baik, komponen tersebut yaitu :

1. Pengirim atau komunikator (sender) adalah pihak yang mengirimkan pesan kepada pihak lain.
2. Pesan (message) adalah isi atau maksud yang akan disampaikan oleh satu pihak kepada pihak lain.
3. Saluran (channel) adalah media dimana pesan disampaikan kepada komunikan. dalam komunikasi antar-pribadi (tatap muka) saluran dapat berupa udara yang mengalirkan getaran nada/suara.
4. Penerima atau komunikate (receiver) adalah pihak yang menerima pesan dari pihak lain
5. Umpan balik (feedback) adalah tanggapan dari penerimaan pesan atas isi pesan yang disampaikannya.

### Contoh-contoh protokol komunikasi yang umum digunakan :

1. TCP/IP (Transmission Control Protocol/Internet Protocol) :
    - TCP (Transmission Control Protocol): TCP adalah protokol yang digunakan untuk mengelola pengiriman data yang handal dalam jaringan. Ini memastikan bahwa data yang dikirimkan dari satu perangkat ke perangkat lainnya sampai dengan benar dan dalam urutan yang tepat.
    - IP (Internet Protocol): IP adalah protokol yang digunakan untuk mengarahkan dan mengirimkan paket data melalui jaringan. IP memungkinkan perangkat untuk diberikan alamat IP yang unik sehingga data dapat dikirim ke tujuan yang benar.
2. HTTP/HTTPS (Hypertext Transfer Protocol/Secure Hypertext Transfer Protocol) :
a.HTTP : HTTP adalah protokol yang digunakan untuk mengirimkan data dalam bentuk dokumen atau halaman web dari server ke peramban web. Ini adalah protokol dasar yang digunakan untuk World Wide Web.
b.HTTPS : HTTPS adalah versi aman dari HTTP yang menggunakan enkripsi SSL/TLS untuk melindungi privasi data saat data dikirimkan antara peramban dan server web.
3. SMTP (Simple Mail Transfer Protocol) : SMTP adalah protokol yang digunakan untuk mengirimkan email. Ini mendefinisikan cara email dikirim dari server pengirim ke server penerima.
4. POP3 (Post Office Protocol version 3) dan IMAP (Internet Message Access Protocol) : Ini adalah protokol yang digunakan oleh klien email untuk mengambil email dari server email. POP3 mendownload email ke perangkat klien, sedangkan IMAP memungkinkan akses yang lebih interaktif dan penyimpanan email di server.
5. FTP (File Transfer Protocol) : FTP adalah protokol yang digunakan untuk mengirimkan file antara dua perangkat dalam jaringan. Ini sering digunakan untuk mengelola dan mentransfer file di antara server dan klien.
6. DNS (Domain Name System) : DNS adalah protokol yang digunakan untuk menerjemahkan nama domain menjadi alamat IP. Ini memungkinkan penggunaan nama domain yang mudah diingat daripada harus mengingat alamat IP numerik.
7. SNMP (Simple Network Management Protocol) : SNMP adalah protokol yang digunakan untuk mengelola dan memantau perangkat jaringan, seperti router, switch, dan printer, dengan mengumpulkan informasi dan mengirimkannya ke manajemen jaringan.
8. MQTT (Message Queuing Telemetry Transport) : MQTT adalah protokol berbasis pesan yang digunakan untuk komunikasi antara perangkat IoT (Internet of Things) dan server. Ini ringan dan efisien dalam mengirimkan data dalam lingkungan terdistribusi.

Setiap protokol memiliki karakteristik dan kegunaan yang berbeda sesuai dengan tujuannya. Penggunaan protokol yang tepat sangat penting dalam memastikan komunikasi yang efisien dan aman dalam jaringan dan sistem komunikasi yang beragam.

## II. Middleware

Middleware dalam sistem terdistribusi adalah perangkat lunak atau lapisan perangkat lunak yang berada di antara perangkat keras (hardware) dan aplikasi (software) dalam sistem terdistribusi. Fungsinya adalah untuk memfasilitasi dan mengelola komunikasi, koordinasi, dan integrasi antara berbagai komponen atau entitas yang terdistribusi dalam suatu jaringan atau lingkungan terdistribusi. Middleware bertindak sebagai perantara yang membantu berbagai komponen dalam sistem untuk berinteraksi dan beroperasi bersama.

### Peran dan fungsi utama middleware dalam sistem terdistribusi

1. Abstraksi Jaringan: Middleware menyediakan abstraksi atas jaringan komunikasi fisik. Ini memungkinkan aplikasi untuk berkomunikasi tanpa perlu tahu detail teknis tentang bagaimana data dikirimkan antara node-node dalam jaringan. Middleware mengelola protokol komunikasi, deteksi kesalahan, dan pemulihan kesalahan secara otomatis.
2. Manajemen Transaksi: Middleware dapat mendukung manajemen transaksi dalam lingkungan terdistribusi. Ini berarti bahwa jika beberapa operasi terjadi di beberapa node, middleware dapat memastikan konsistensi data dengan mengelola komit atau rollback transaksi sesuai kebutuhan.
3. Distribusi dan Replikasi Data: Middleware dapat membantu dalam mendistribusikan data di seluruh sistem terdistribusi dan mengelola replikasi data untuk keandalan dan kinerja. Hal ini penting untuk sistem yang memiliki banyak node yang harus bekerja dengan data yang sama.
4. Pemantauan dan Manajemen Kinerja: Middleware sering menyertakan alat-alat untuk pemantauan dan manajemen kinerja sistem terdistribusi. Ini memungkinkan administrator untuk melacak kinerja sistem, memecahkan masalah, dan melakukan tindakan pengelolaan jika diperlukan.
5. Keamanan: Middleware dapat menyediakan lapisan keamanan untuk melindungi komunikasi dan data dalam sistem terdistribusi. Ini termasuk autentikasi, otorisasi, enkripsi, dan kontrol akses.
6. Skalabilitas: Middleware dapat membantu sistem untuk menjadi lebih mudah diubah dan ditingkatkan. Ini dapat mencakup kemampuan untuk menambahkan atau menghapus node dengan mudah dan mengatasi pertumbuhan sistem yang besar.
7. Pengiriman Pesan dan Sinyal: Middleware sering digunakan dalam sistem berbasis pesan (message-based) atau sistem yang menggunakan sinyal atau peristiwa (event-based) untuk berkomunikasi antara komponen. Middleware dapat mengelola antrian pesan, pembuatan peristiwa, dan pengiriman pesan atau sinyal ke penerima yang tepat.

### Contoh Middleware

1. CORBA (Common Object Request Broker Architecture)
2. RMI (Remote Method Invocation) untuk Java
3. Message queuing middleware seperti Apache Kafka dan RabbitMQ.

Penggunaan middleware dalam sistem terdistribusi dapat mengurangi kompleksitas pengembangan aplikasi, memungkinkan integrasi yang lebih baik antara komponen yang berbeda, dan memastikan kinerja, keandalan, dan keamanan komunikasi dalam lingkungan terdistribusi yang kompleks.
