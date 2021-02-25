# Fragment

Fragment merupakan kombinasi sebuah layout XML dan kelas java yang mirip dengan sebuah Activity yang memiliki fungsi untuk menampilkan antarmuka ke pengguna. Dengan menggunakan support library, fragment dapat mendukung hampir semua versi Android. Fragment digunakan agar komponen tampillan aplikasi menjadi fleksibel dan dapat digunakan kembali ( reusable). Fragment merupakan komponen utuh yang memiliki view, event, dan logic (meskipun tetap membutuhkan sebuah fragment agar dapat bekerja).

Fragment juga bisa disebut sub nya activity (Sebuah fragment harus berada di dalam sebuah activity, mereka tidak dapat berjalan sendiri tanpa adanya activity tempat mereka menempel). Dalam satu activity bisa memiliki lebih dari satu fragment.

# Pentingnya Sebuah Fragment

1.	Penggunaan Komponen View dan Logic Berulang Kali : Fragment dapat dipakai untuk menampilkan data atau melakukan event tertentu dibeberapa activity berbeda.
2.	Dukungan Untuk Tablet : Fragment memungkinkan activity untuk menggunakan fragment dalam membuat antarmuka sesuai dengan perangkat yang membukanya.
3.	Orientasi Layar : Fragment memungkinkan  untuk menggunakan tampilan yang berbeda( horizontal atau vertikal) menggunakan elemen yang sama.

# Keuntungan Menggunakan Fragmen 

1.Tidak perlu memasukkan nama file fragment ke dalam “AndroidManifest” yang diperlukan oleh activity.

2.Fungsi yang berada pada activity dapat langsung digunakan dalam fragment tersebut tanpa harus membuat ulang. 

# Fragment Lifecyle

Fragment memiliki sirkulasi kehidupan atau yang biasanya disebut “lifecycle”, seperti yang ditunjukkan pada Gambar  di bawah ini :

![fragnen](https://user-images.githubusercontent.com/60412314/109186437-7fb79d80-77c3-11eb-9f44-bb54e2175e16.jpg)

1. onAttach() dipanggil saat sebuah fragment terhubung ke activity.
2. onCreate() diapnggil saat sebuah fragment dibuat (objeknya di memori).
3. onCreateView() dipanggil saat fragment sudah siap membaca sebuah layout.
4. onViewCreated() dipanggil setelah onCreateView() dan memastikan layout yang dibaca fragment adalah non-null. Semua pengaturan view seperti pembacaan findViewById, menambah onClickListener dapat dilakukan di sini.
5. onActivityCreated() dipanggil setelah activity pembaca sudah menyelesaikan onCreate()-nya.
6. onStart() dipanggil setelah fragment siap untuk ditampilkan di layar.
7. onResume() - Dipakai untuk melakukan pembacaan data yang lebih “rumit” seperti lokasi, sensor, dll.
8. onPause() - Tempat melepas data “rumit”. Lakukan commit di sini.
9. onDestroyView() dipanggil saat layout sebuah fragment akan dihapus dari memori, namun fragmentnya masih ada di memori.
10.onDestroy() dipanggil jika fragment sudah tidak dipakai.
11. onDetach() dipanggil saat fragment tidak lagi terhubung ke sebuah activity.

# Pembuatan Sebuah Fragment

Sebuah fragment, seperti activity, memiliki XML layout-nya sendiri dan sebuah kelas java sebagai controller dari Fragment tersebut.Layout XML yang dimiliki oleh fragment, sama seperti layout-layout lainnya dan bisa memiliki nama apa saja (selama memiliki format yang ditentukan). 

# Penerapaan Fragment

![WhatsApp Image 2021-02-25 at 23 31 43](https://user-images.githubusercontent.com/60412314/109184798-e936ac80-77c1-11eb-85ad-ca3498ecd32d.jpeg)
![WhatsApp Image 2021-02-25 at 23 31 48](https://user-images.githubusercontent.com/60412314/109184812-eb990680-77c1-11eb-9d9c-a4422e34b724.jpeg)

Sumber yang di ambil [ Selengkapnya...](https://https://www.codepolitan.com/membuat-dan-menggunakan-fragment-59f80eff061a4)

## TERIMAKSIH :)
