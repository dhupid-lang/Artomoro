# ARTOMORO KASIR — Android Studio starter project

Versi prototipe 0.2.0 untuk toko alat kesehatan dan layanan servis. Antarmuka Indonesia dibungkus dengan Android WebView, dengan penyimpanan lokal pada perangkat.

## Fitur prototipe
- Login lokal demo untuk peran admin dan kasir.
- Admin: produk/stok, laporan, backup/restore; kasir: transaksi.
- Tambah produk, kode/barcode teks, harga modal/jual dan stok.
- Keranjang, validasi stok, diskon, pajak, pelanggan, transaksi dan omzet hari ini.
- Struk transaksi dengan dialog cetak; hasil cetak bergantung pada dukungan Android/layanan cetak yang terpasang.
- Filter tanggal laporan dan ekspor CSV yang dapat dibuka di Excel.
- Backup dan pemulihan JSON lokal.

## Akun demo
- Admin: `admin` / `admin123`
- Kasir: `kasir` / `kasir123`

**Penting:** kredensial ini hanya untuk demo, bukan keamanan produksi. Ganti sebelum dipakai sungguhan. Data tersimpan di perangkat dan tidak dienkripsi. Jangan jadikan satu-satunya catatan transaksi.

## Belum tersedia / perlu pengembangan dan pengujian
- Login aman dengan pengelolaan akun/PIN dan audit transaksi.
- Scan barcode langsung dari kamera (input kode teks atau scanner keyboard dapat digunakan saat ini).
- Integrasi printer thermal Bluetooth ESC/POS langsung; cetak sekarang memakai dialog cetak Android/WebView.
- Sinkronisasi otomatis Google Drive/cloud.
- File Excel XLSX dan PDF laporan yang terformat (ekspor saat ini CSV).
- Pengujian pada perangkat Android dan uji pemulihan data.

## Membuat APK
1. Instal Android Studio dan Android SDK Platform 35.
2. Buka folder `ArtomoroKasir` di Android Studio.
3. Tunggu Gradle Sync selesai (perlu internet saat mengunduh plugin/dependensi jika belum tersedia).
4. Pilih **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. APK debug biasanya berada di `app/build/outputs/apk/debug/app-debug.apk`.

Paket ini berisi source project, **bukan APK terkompilasi**. Lingkungan ini tidak menyediakan Android SDK/Gradle untuk mengompilasi dan menguji APK secara langsung.


Versi 0.5.0: menu Dokumen PDF menambahkan pembuatan Surat Penawaran Harga dan Invoice Penagihan dengan logo ARTOMORO FILTER. Rekening Bank Mandiri ditampilkan hanya pada invoice. Pilih Cetak lalu Save as PDF. Nomor dan nama pemilik rekening masih placeholder dan wajib dilengkapi sebelum invoice dikirim.
