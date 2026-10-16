<!-- Deskripsi Skenario -->
Mahasiswa mengajukan KRS dengan memilih mata kuliah. Setiap
pengajuan menjalankan validasi KRS yang memeriksa kelengkapan,
prasyarat mata kuliah, dan benturan jadwal. Jika validasi berhasil,
sistem menyimpan pengajuan berstatus menunggu persetujuan dosen
wali. Pada konfirmasi penyimpanan, mahasiswa dapat memilih
mengunduh bukti pengajuan. Dosen wali menyetujui atau menolak KRS
dan memberikan catatan keputusan.

<!-- Tabel Kebutuhan -->
|  ID   |                             Kebutuhan_tugas                              |
|-------|--------------------------------------------------------------------------|
|SIA-R01|                  Mahasiswa dapat melihat jadwal kuliah                   |
|SIA-R02|               Admin akademik dapat mengelola jadwal kuliah               |
|SIA-R03|                      Mahasiswa dapat mengajukan KRS                      |
|SIA-R04|             Sistem memvalidasi KRS sebagai bagian pengajuan              |
|SIA-R05|Mahasiswa dapat mengunduh bukti jika memilihnya pada konfirmasi pengajuan |
|SIA-R06|        Dosen wali dapat memproses persetujuan atau penolakan KRS         |

<!-- Batas dan Asumsi -->
Batas dan asumsi:
• Pengguna telah terautentikasi.
• Data mata kuliah, prasyarat, dan jadwal tersedia.
• Validasi gagal menyebabkan pengajuan belum berhasil tersimpan.
• Unduh bukti tidak menjadi syarat keberhasilan pengajuan.
• KRS tersimpan belum berarti disetujui.
• Pembayaran, pengisian nilai, dan implementasi basis data berada di luar tugas.

<!-- Tabel Identifikasi Aktor -->
|    Aktor     |                Tujuan_terhadap_sistem                 |
|--------------|-------------------------------------------------------|
|  Mahasiswa   |Mengajukan KRS, Melihat Jadwal Kuliah, Mengunduh Bukti |
|Admin_Akademik|                 Kelola Jadwal Kuliah                  |
|  Wali_Dosen  |                  Memproses Keputusan                  |

<!-- Tabel Susuna Katalog use Case -->
|  ID   |   Nama_use_case    |      Peran_dalam_model      |
|-------|--------------------|-----------------------------|
|SIA-R03|     Ajukan_KRS     |   Fungsi Utama Mahasiswa    |
|SIA-R01|Lihat_Jadwal_Kuliah |   Fungsi Utama Mahasiswa    |
|SIA-R05|    Unduh_Bukti     |Perilaku yang disertakan R03 |
|SIA-R02|Kelola_Jadwal_Kuliah| Fungsi Utama Admin Akademik |
|SIA-R06|Proses_Keputusan_KRS|   Fungsi Utama Dosen Wali   |

<!-- Relasi Include -->

<!-- Relasi Extand -->