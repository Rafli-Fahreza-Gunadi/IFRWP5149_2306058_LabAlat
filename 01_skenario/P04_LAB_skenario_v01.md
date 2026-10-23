Skenario berikut merupakan bahan latihan yang ditetapkan untuk
jobsheet, bukan hasil pengumpulan kebutuhan laboratorium nyata.
Skenario ini melanjutkan potongan model Pertemuan 3.
Selain mahasiswa, dosen juga meminjam peralatan laboratorium untuk
kegiatan praktikum dan penelitian. Mahasiswa dan dosen sama-sama
dapat melihat ketersediaan peralatan dan mengajukan peminjaman.
Petugas laboratorium mengelola data peralatan: menambah peralatan
baru, mengubah data peralatan, dan menghapus data peralatan yang
tidak lagi dipakai. Setelah peminjaman disetujui dan alat diambil, petugas
mencatat pengembalian peralatan. Pada saat mencatat pengembalian,
petugas memeriksa dan mencatat kondisi peralatan. Dua use case utama
pada potongan model ini, Ajukan Peminjaman dan Catat Pengembalian
Peralatan, ditunjukkan realisasinya oleh collaboration yang bersesuaian.
Seluruh fungsi Pertemuan 3 tetap berlaku dan tetap digambar:
pemeriksaan ketersediaan di dalam pengajuan, pencetakan bukti
pengajuan oleh mahasiswa, proses keputusan peminjaman oleh petugas,
dan laporan peminjaman untuk kepala laboratorium. Diagram Pertemuan
4 adalah diagram Pertemuan 3 yang ditambah, bukan diagram baru yang
menggantikannya.

|       Aktor        |                 Kedudukan                  |                                                            Tujuan_terhadap_sistem                                                             |
|--------------------|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
|      Peminjam      |   Umum_(general),_baru_pada_Pertemuan_4    |                             Peran_umum bagi peminjam peralatan. Mewariskan fungsinya kepada Mahasiswa dan Dosen.                              |
|     Mahasiswa      |Khusus_dari_Peminjam,_tetap_dari_Pertemuan_3|Melihat_ketersediaan dan mengajukan peminjaman (diwarisi dari Peminjam), ditambah mencetak bukti pengajuan sebagai asosiasi khususnya sendiri. |
|       Dosen        |Khusus_dari_Peminjam,_baru_pada_Pertemuan_4 |                                   Melihat_ketersediaan dan mengajukan peminjaman (diwarisi dari Peminjam).                                    |
|Petugas_Laboratorium|           Tetap_dari_Pertemuan_3           |                        Mengelola data peralatan, memproses keputusan peminjaman, dan mencatat pengembalian peralatan.                         |
|Kepala_Laboratorium |           Tetap_dari_Pertemuan_3           |                                                          Melihat laporan peminjaman.                                                          |

