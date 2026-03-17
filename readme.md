🌍 Terralnvest
Terralnvest adalah platform web interaktif yang mengedukasi dan mengajak pengguna untuk peduli terhadap masa depan planet melalui investasi pada upaya konservasi lingkungan. Website ini menampilkan dampak nyata dari konservasi serta menyediakan informasi mendalam tentang ekosistem dunia.
🏆 Dibuat untuk mengikuti Lomba Web Design.

📋 Daftar Isi
- Tentang Project
- Fitur Utama
- Teknologi yang Digunakan
- Screenshot
- Struktur File
- Instalasi & Menjalankan Project
- Deployment
- Tim Pengembang
- Referensi & Aset

📖 Tentang Project
Terralnvest lahir dari keprihatinan terhadap krisis iklim dan hilangnya habitat kritis di seluruh dunia. Website ini bertujuan untuk:

1. Mengedukasi masyarakat tentang pentingnya ekosistem dan dampak krisis iklim
2. Menginspirasi aksi nyata melalui proyek-proyek konservasi
3. Menghubungkan pengguna dengan upaya restorasi lingkungan

Website ini didesain dengan dua tampilan utama:
- Halaman Beranda (Landing Page): Menampilkan masalah, solusi, dampak sosial, dan ajakan untuk bergabung. Dilengkapi dengan fitur Dark Mode untuk kenyamanan pengguna.

- Halaman Edukasi (Ecosystems): Menyajikan 12 slide materi tentang ekosistem dengan format horizontal scroll yang interaktif dan informatif.

🛠️ Teknologi yang Digunakan
Teknologi	
Laravel 10	        :Framework PHP untuk backend & routing
HTML5	            :Struktur halaman
CSS	                :Styling, grid, flexbox, animasi
JavaScript 	        :Interaktivitas (dark mode, navigasi slide)
Local Storage	    :Menyimpan preferensi tema pengguna
Responsive Design	:Tampilan optimal di desktop, tablet, dan HP

📁 Struktur File
text
terralnvest/
├── app/
│   └── Http/
│       └── Controllers/
│           ├── HomeController.php       # Controller halaman utama
│           └── EcosystemController.php  # Controller halaman edukasi
├── resources/
│   └── views/
│       ├── home.blade.php               # Halaman beranda
│       ├── layouts/
│       │   └── app.blade.php            # Layout utama (navbar, toggle)
│       └── ecosystems/
│           └── index.blade.php          # 12 slide horizontal
├── public/
│   ├── css/
│   │   ├── style.css                    # CSS halaman beranda
│   │   └── ecosystems.css               # CSS halaman slide
│   ├── js/
│   │   └── ecosystems.js                # JavaScript navigasi slide
│   └── images/                           # Gambar aset
│       ├── bg1.jpg                       # Hero background
│       ├── bernea-omigtan.jpg
│       ├── sanctuary.jpg
│       ├── raja-amgo.jpg
│       └── raja-anas-dik.jpg
├── routes/
│   └── web.php                          # Daftar route
├── .env                                  # Konfigurasi environment
├── .gitignore
├── artisan
├── composer.json
└── README.md                             # File ini

⚙️ Instalasi & Menjalankan Project
Prasyarat
PHP >= 8.1
Composer
Git
Langkah Instalasi
Clone repositori
git clone https://github.com/AdamMR12/kobers.git
cd kobers

Install dependensi PHP
composer install
Konfigurasi environment

🌐 Deployment
GitHub Pages (Static)
# Install package export
composer require spatie/laravel-export --dev

# Export ke folder public/export
php artisan export

# Upload folder export ke GitHub Pages
cd public/export
git init
git add .
git commit -m "Static version"
git remote add origin https://github.com/AdamMR12/kobers.git
git push -u origin main
Live Demo (GitHub Pages): https://AdamMR12.github.io/kobers

👥 Tim Pengembang
Haikal	UI/UX Designer	
Adam	Backend & Frontend Developer	
Nizar   Dokumenter
Universitas/Sekolah: [Politeknik Negeri Subang]
Tim: [kober]

🎨 Desain & Konsep Visual
Warna Utama
Warna	    |Light Mode	|Dark Mode	|Penggunaan
Hijau	     #4CAF50	 #6ab04c	 Aksen, tombol, statistik
Putih/Abu	 #ffffff	 #1a1a1a	 Background utama
Abu Teks	 #666666	 #cccccc	 Teks sekunder

Tipografi
Font Utama: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto
Ukuran Judul: 3.5rem (desktop), 2rem (tablet), 1.8rem (HP)
Ukuran Teks: 1.2rem (desktop), 1rem (tablet), 0.85rem (HP)

Responsive Breakpoints
Device	    |Max Width	    |Grid Kolom
Desktop	     >1200px	     4 kolom
Tablet	     992px - 1200px	 2 kolom
HP Landscape 768px - 992px	 2 kolom
HP Portrait	 480px - 768px	 1-2 kolom
HP Kecil	 <480px	         1 kolom

🚀 Fitur Unggulan
1. Horizontal Scroll dengan Snap
.slides-container {
    scroll-snap-type: x mandatory;
    scroll-behavior: smooth;
}
.slide {
    scroll-snap-align: start;
}

2. Responsive Terrestrial Cards
Desktop: 4 kolom
Tablet: 2 kolom
HP: 1 kolom dengan layout flex (icon kiri, teks kanan)

3. Energy Flow Animasi
Flow item dengan background transparan
Panah animasi di desktop, rotate 90° di HP

📝 Catatan Pengembangan
Tantangan & Solusi
Tantangan	            |Solusi
Teks mentok di HP	     word-wrap: break-word, overflow-wrap: break-word
Navbar nutup konten	     padding-top di slide sesuai tinggi navbar
Dark mode konsisten	     CSS Variables + Local Storage
Horizontal scroll di HP	 Touch events + JavaScript

Optimasi
Semua gambar dikompres < 200KB
CSS dan JS di-minify untuk production
Menggunakan laravel-export untuk static hosting

🙏 Referensi & Aset
Desain
Desain UI/UX oleh tim
Ikon & Emoji
Menggunakan emoji universal untuk ikon (🌱, ☀️, 🌊, dll)
Kompatibel di semua browser dan device
Konten Edukasi
Diadaptasi dari berbagai sumber terbuka tentang ekologi:
National Geographic
WWF (World Wildlife Fund)
Encyclopedia Britannica
Modul Biologi SMA/Universitas
Kode & Library
Laravel Documentation
CSS Tricks - Guide to Flexbox
CSS Tricks - Guide to Grid
Inspirasi README dari Best-README-Template

📞 Kontak
Untuk pertanyaan lebih lanjut, hubungi:

Email: adammr126@gmail.com
GitHub: github.com/AdamMR12/kobers

📄 Lisensi
© 2026 kobers Team. All rights reserved.
Project ini dibuat untuk tujuan lomba dan pendidikan. Dilarang memperbanyak untuk tujuan komersial tanpa izin.

🏆 Penutup
"Kita tidak mewarisi Bumi dari nenek moyang kita, kita meminjamnya dari anak cucu kita."
— Peribahasa Suku Asli Amerika

Terima kasih telah mengunjungi project Terralnvest. Semoga website ini dapat menginspirasi aksi nyata untuk masa depan planet kita! 🌍💚

🔗 Live Demo: https://adammr12.github.io/kobers/
📂 Repository: https://github.com/AdamMR12/kobers

README ini terakhir diperbarui: 17 Maret 2026
