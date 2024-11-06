# JOBSHEET 9 Tugas Praktikum 

Nama: Wulan Maulidya P. F

Kelas: TI-3H

No. Absen: 27

NIM: 2241720174

---

## Gabungkan hasil praktikum 1 dengan hasil praktikum 2 sehingga setelah melakukan pengambilan foto, dapat dibuat filter carouselnya!

**Tambah Dependensi**

![Tugas](/images/1a.png)

**lib/widget/kamera/takepicture_screen.dart**

![Tugas](/images/1b.png)

**lib/widget/kamera/displaypicture_screen.dart**

![Tugas](/images/1c.png)

**lib/widget/filter/filter_selector.dart**

![Tugas](/images/1d.png)

**lib/widget/filter/filter_carousel.dart**

![Tugas](/images/1e.png)

**lib/widget/filter/carousel_flowdelegate.dart**

![Tugas](/images/1f.png)

**lib/widget/filter/filter_item.dart**

![Tugas](/images/1g.png)

**lib/main.dart**

![Tugas](/images/1h.png)

**Output:**

![Tugas](/images/1i.gif)

## Jelaskan maksud void async pada praktikum 1?
Praktikum 1: lib/main.dart
![Tugas](/images/2.png)

* void async mendeklarasikan bahwa function tersebut adalah asynchronous. Function asynchronous membuat kode menjalankan tugas-tugas yang membutuhkan waktu tanpa menghentikan eksekusi program secara keseluruhan.

* Pada kode tersebut, main() dideklarasikan sebagai async yang berarti function ini bisa menjalankan operasi yang membutuhkan waktu seperti await availableCameras();, yaitu menunggu daftar kamera yang tersedia. Penggunaan await memblokir sementara eksekusi kode berikutnya hingga daftar kamera selesai diambil, tetapi tidak menghentikan keseluruhan program (program tetap bisa menjalankan tugas lain yang tidak bergantung pada await tersebut).

* Sehingga, void async mengizinkan main() untuk melakukan tugas asynchronous tanpa mengembalikan nilai apa pun dan membuat program berjalan secara efisien tanpa menunggu setiap operasi selesai secara langsung.

## Jelaskan fungsi dari anotasi @immutable dan @override?
Praktikum 2: lib/widget/filter_selector.dart
![Tugas](/images/3.png)

* @immutable: Anotasi @immutable digunakan untuk menandai bahwa sebuah kelas bersifat immutable, yang berarti bahwa setelah objek dibuat, semua properti atau atributnya tidak dapat diubah. Pada kode tersebut, FilterSelector diberi anotasi @immutable, yang berarti setiap instance FilterSelector harus dibuat dengan semua nilai propertinya yang sudah tetap (tidak dapat diubah) setelah konstruktor dijalankan. @immutable digunakan untuk mencegah bug yang muncul karena perubahan state yang tidak terduga, dan membuat kode lebih mudah dipahami.

* @override: Anotasi @override digunakan ketika sebuah metode dari kelas induk (superclass) di-override atau ditimpa dalam subclass (kelas turunan).Pada kode tersebut, @override digunakan pada method createState dalam FilterSelector yang menandakan bahwa createState sedang meng-override metode createState dari superclass StatefulWidget. @override digunakan untuk memastikan method diimplementasikan sesuai dengan deklarasi pada superclass, dan membantu mendeteksi kesalahan ketika nama method salah ketik atau tidak sesuai dengan superclass.