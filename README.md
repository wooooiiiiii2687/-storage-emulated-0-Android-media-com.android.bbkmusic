Peran teknologi dalam segala sistem Bisines
Aplikasi
Memberikan informasi penjual Anda dengan sellers.json
Berikutnya: Transparansi bid dengan objek SupplyChain
Sellers.json adalah standar IAB Tech Lab yang meningkatkan transparansi dalam ekosistem iklan dan membantu memerangi penipuan. Sellers.json berfungsi melalui file informasi penjual yang tersedia secara publik. Penayang dapat memilih untuk memberikan informasi penjualnya di file tersebut. Tindakan ini memberikan cara yang andal bagi pengiklan untuk menemukan dan memverifikasi identitas penayang.

Secara default, hanya ID penjual Anda yang dicantumkan di file sellers.json. Sebaiknya buat informasi yang transparan dan izinkan nama bisnis Anda untuk dicantumkan juga. Dengan begitu, pengiklan dapat memverifikasi inventaris Anda. Jika informasi Anda tidak transparan, pengiklan tidak akan dapat melihat nama bisnis Anda, sehingga memengaruhi pendapatan Anda. 

Catatan: Perlu waktu hingga 7 hari agar file sellers.json diperbarui dengan informasi penjual Anda.

Perhatikan juga bahwa tidak semua domain dapat ditambahkan, kecuali jika domain tersebut dapat diverifikasi.

Kolom sellers.json
File sellers.json menyertakan kolom berikut:

Kolom	Deskripsi
seller_id	16 digit kode penayang, mis. pub-0000000000000000
is_confidential	Jika ditetapkan ke benar, nama dan domain tidak akan dicantumkan di file sellers.json.
seller_type	PENAYANG atau PERANTARA atau KEDUANYA. Jika Anda adalah pemilik aplikasi yang Anda monetisasi dan/atau Anda dibayar langsung oleh Google, Anda diklasifikasikan sebagai PENAYANG. Jika tidak, Anda akan diklasifikasikan sebagai PERANTARA. Jika Anda termasuk dalam kedua kategori tersebut, Anda akan diklasifikasikan sebagai KEDUANYA.
nama	
Nama penjual Anda. Ini adalah nama yang ditampilkan di bagian Nama dan alamat pada profil pembayaran Anda di AdMob. 

Untuk melihat profil pembayaran Anda, klik Pembayaran di sidebar lalu klik Kelola setelan. 

Catatan: Jika Anda mengubah nama bisnis, pembayaran otomatis akan tertunda selama dua minggu.
domain	
Domain bisnis Anda (mis. example.com) jika ada. Jika bisnis Anda tidak memiliki kehadiran di internet, kolom ini boleh tidak diisi.

Jika Anda adalah PERANTARA, ini adalah domain tempat file sellers.json dapat ditemukan.

Pelajari domain bisnis lebih lanjut.

Cara membuat informasi penjual menjadi transparan
Login ke akun AdMob Anda di https://admob.google.com.
Klik Setelan di sidebar.
Klik tab Akun.
Di bagian "Kontrol akun", klik Edit di samping Informasi penjual (sellers.json):
Pilih Transparan.
(Opsional) Tambahkan domain bisnis Anda, lalu klik Verifikasi. 
Klik Simpan. 
Nama, domain bisnis (jika ada), dan ID penayang Anda akan muncul di file sellers.json Google. Nama di profil penagihan Anda adalah nama yang akan ditampilkan kepada pengiklan. Jika ingin mengganti nama di profil penagihan, sebaiknya lakukan setelah siklus penagihan. Perubahan pada profil penagihan akan menyebabkan pembayaran otomatis tertunda selama dua minggu.

Contoh
 
Dalam contoh ini, penayang telah membuat informasinya terlihat di file sellers.json Google. Berikut ini yang dilihat pengiklan:
 
"seller_id": "pub-0000000000000000",
"seller_type": "PENAYANG",
"nama": "Contoh Perusahaan Inc."
Domain bisnis Anda
Domain bisnis Anda merupakan domain untuk entitas perusahaan Anda, bukan domain tempat inventaris dimonetisasi.

Nama domain bisnis Anda mungkin tersembunyi di seller.json hingga kami memverifikasi bahwa Anda adalah pemilik URL. Domain bisnis Anda juga dapat dihilangkan jika akun Anda disetel ke rahasia atau jika bisnis Anda tidak memiliki situs.

Gunakan domain root. Nama domain tidak boleh menyertakan “www” atau skemanya (yaitu, “https://”, “http://”, atau “ftp://”). Domain Anda harus menggunakan akhiran publik. Domain level teratas tidak boleh didahului dengan titik.

 	Kasus penggunaan	Contoh
Didukung	Nama domain	google.com dan google.co.uk
Tidak didukung	Skema	https://google.com
Tidak didukung	Awalan dan subdomain	www.google.com dan subdomain.google.com
Tidak didukung	Garis miring	google.com/
Tidak didukung	Suffix domain yang tidak didukung	google.ltd dan google.tech
Transparansi perantara 
Akun dengan jenis penjual PERANTARA menjual inventaris di Google Ad Manager yang tidak dimiliki oleh akun tersebut atau tidak dibayar langsung oleh Google. Misalnya, penayang induk Pengelolaan Banyak Pelanggan akan memenuhi syarat sebagai perantara.

Untuk perantara dan akun dengan jenis penjual KEDUANYA, kolom is_confidential akan ditetapkan ke salah secara default.

Informasi Anda di file sellers.json Google
Tinjau file sellers.json Google di realtimebidding.google.com/sellers.json.

Jika memiliki satu atau beberapa akun dengan AdSense, AdMob, atau Ad Manager, Anda akan muncul di sellers.json untuk setiap produk. seller_id Anda bersifat unik untuk setiap produk, tetapi status transparansi dan domain Anda akan sama di semua produk. Status Anda tidak mungkin dirahasiakan untuk satu produk dan ditampilkan di produk lainnya.

Jika Anda mengedit informasi bisnis untuk sellers.json di AdSense, AdMob, atau Ad Manager, informasi Anda akan diperbarui di semua produk. Misalnya, jika Anda membuka akun AdSense dan mengaktifkan transparansi Seller.json, tindakan ini juga akan otomatis mengaktifkan transparansi pada akun Ad Manager dan AdMob Anda.

"Nama domain bisnis Anda mungkin tersembunyi di seller.json hingga kami memverifikasi bahwa Anda adalah pemilik URL. Domain bisnis Anda juga dapat dihilangkan jika akun Anda disetel ke rahasia atau jika bisnis Anda tidak memiliki situs"
Perusahaan Contoh Inc. mengaktifkan transparansi di akun Ad Manager . Akun AdMob dan akun AdSense Perusahaan Contoh Inc. akan diperbarui secara otomatis untuk mengaktifkan transparansi.

Saat Perusahaan Contoh Inc. memperbarui domain bisnis menjadi example.com di AdSense, akun Ad Manager dan AdMob miliknya akan otomatis diperbarui sehingga juga menyertakan domain bisnis example.com.

Menemukan informasi
Download file sellers.json Google (klik kanan link, lalu klik Simpan Link Sebagai).
Buka file sellers.json yang telah didownload.
Gunakan Ctrl + F (Command ⌘ + F, untuk Mac) untuk menemukan seller_id.
Tinjau informasi Anda.

Perusahaan Contoh Inc.Akun AdMob dan akun AdSense Perusahaan Contoh Inc. akan diperbarui secara otomatis untuk mengaktifkan transparansi.

Saat Perusahaan Contoh Inc. 
memperbarui domain bisnis menjadi example.com di AdSense, akun Ad Manager dan AdMob miliknya akan otomatis diperbarui sehingga juga menyertakan domain bisnis example.com.

Beri masukan tentang artikel ini

Berikutnya: Transparansi bid dengan objek Supply
Apakah ini membantu?
YaTidak
PerSupplylain?
Coba langkah-langkah selanjutnya berikut:
Posting ke komunitas bantuan
Dapatkan jawaban dari anggota komunitas
Hubungi kami
Beri tahu kami selengkapnya dan kami akan membantu Anda
