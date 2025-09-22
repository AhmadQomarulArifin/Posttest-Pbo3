# Posttest-Pbo3

# Program CRUD Klinik Hewan Peliharaan

Deskripsi Program

Program ini adalah manajemen data hewan di klinik yang dibuat dengan bahasa Java menggunakan konsep Object-Oriented Programming (OOP). Aplikasi ini menerapkan encapsulation, inheritance, overriding, dan polymorphism dengan struktur berbasis Model-View-Controller (MVC). Fitur utamanya meliputi CRUD data hewan, validasi input, serta pencarian data. Dengan desain ini, program menjadi rapi, mudah dikembangkan, dan relevan sebagai simulasi manajemen klinik hewan.


### Class






<img width="288" height="189" alt="image" src="https://github.com/user-attachments/assets/fa9dadfe-3271-49a7-b283-de19e93f6bfa" />





Program ini terdiri dari lima class , yaitu class Hewan, Burung, dan Ikan yang berada pada package model, class HewanService pada package service, serta class Main pada package main. Class Hewan berperan sebagai superclass yang menyimpan data umum hewan, sedangkan Burung dan Ikan merupakan subclass yang mewarisi Hewan sekaligus menambahkan atribut serta overriding method tampilkanInfo(). Class HewanService berfungsi sebagai pengelola logika CRUD dan pencarian data hewan, sementara class Main menjadi pengendali utama program yang menampilkan menu interaktif kepada pengguna.





### Properties






<img width="993" height="234" alt="image" src="https://github.com/user-attachments/assets/4239a4fc-cc7b-4fd4-8fdf-34995b814a7f" />







<img width="983" height="135" alt="image" src="https://github.com/user-attachments/assets/2de7f095-1cdf-4ce4-a770-746e29cdaeea" />







<img width="1010" height="137" alt="image" src="https://github.com/user-attachments/assets/98196ac9-389d-4c6c-bbfe-bbc1a98a243f" />









Pada program ini, setiap class memiliki properti yang berbeda sesuai dengan perannya. Class Hewan sebagai superclass memiliki enam properti, yaitu namaPemilik, noHP, namaHewan, jenisHewan, umurHewan, dan keluhan. Properti ini digunakan untuk menyimpan informasi umum tentang hewan yang didaftarkan ke klinik. Subclass Burung menambahkan satu properti baru yaitu warnaBulu, yang merepresentasikan ciri khas burung. Subclass Ikan juga menambahkan satu properti khusus yaitu jenisAir, yang menunjukkan apakah ikan hidup di air tawar atau air laut.







### Constructor







<img width="973" height="160" alt="image" src="https://github.com/user-attachments/assets/633d3ac6-69bb-4625-a025-4bd9efe429ba" />











<img width="1000" height="75" alt="image" src="https://github.com/user-attachments/assets/df886c52-80c8-4fb9-9cd0-93868bf8c701" />









<img width="984" height="86" alt="image" src="https://github.com/user-attachments/assets/c5f57f54-4dcc-4549-85d5-8b44c0f4532c" />








Class Hewan memiliki constructor yang digunakan untuk menginisialisasi enam properti utama, yaitu namaPemilik, noHP, namaHewan, jenisHewan, umurHewan, dan keluhan. Constructor ini memastikan bahwa setiap kali objek hewan dibuat, semua data penting langsung terisi. Subclass Burung juga memiliki constructor yang memanggil constructor superclass (super(...)) untuk mengisi data umum hewan, lalu menambahkan inisialisasi properti khusus yaitu warnaBulu, sedangkan subclass Ikan, di mana constructor-nya memanggil constructor Hewan untuk data umum dan menambahkan pengisian properti jenisAir.








### Access Modifier






<img width="604" height="71" alt="image" src="https://github.com/user-attachments/assets/d40d1619-a1de-47b1-829a-c7930837becf" />








<img width="316" height="54" alt="image" src="https://github.com/user-attachments/assets/11c7871b-baa4-4149-8f6a-d005b492bade" />









<img width="287" height="56" alt="image" src="https://github.com/user-attachments/assets/c9e7ad07-c10e-4038-8a7d-ecbe13b47990" />








<img width="683" height="350" alt="image" src="https://github.com/user-attachments/assets/174ea7c5-5010-4d24-850f-fce32bed644c" />





<img width="458" height="114" alt="image" src="https://github.com/user-attachments/assets/4d7efc90-99e6-4a56-a9b8-bfc97179ed79" />






<img width="699" height="149" alt="image" src="https://github.com/user-attachments/assets/3d0dfa41-8227-48fc-9147-01f1741326b5" />





Pada program Klinik Hewan, seluruh atribut pada class Hewan, Burung, dan Ikan menggunakan access modifier private untuk menjaga prinsip encapsulation sehingga data tidak dapat diakses langsung dari luar class. Akses terhadap data dilakukan melalui getter dan setter yang bersifat public, sehingga tetap aman namun fleksibel. Method CRUD pada class HewanService juga menggunakan public agar dapat dipanggil dari class Main, sementara method tampilkanInfo() dibuat public agar bisa dioverride di subclass dan diakses dari luar.







### Struktur packages








<img width="290" height="181" alt="image" src="https://github.com/user-attachments/assets/d3a417b6-1b17-4671-85b6-b2f7e3c99e25" />









Program Klinik Hewan ini disusun menggunakan konsep package untuk memisahkan class berdasarkan fungsinya agar kode lebih terstruktur dan mudah dipahami. Package model berisi class yang merepresentasikan data, yaitu Hewan sebagai superclass serta Burung dan Ikan sebagai subclass yang menambahkan atribut khusus dan melakukan overriding method. Package service berisi class HewanService yang mengatur logika bisnis, terutama operasi CRUD dan pencarian data. Sementara itu, package main berisi class Main yang menjadi titik awal program, menampilkan menu interaktif, dan memanggil method dari service.








## MVC






<img width="287" height="187" alt="image" src="https://github.com/user-attachments/assets/4df419db-f501-4e09-846f-d3e4ba1ff415" />









Program Klinik Hewan ini menerapkan pola Model–View–Controller (MVC) untuk memisahkan struktur kode berdasarkan fungsinya. Model direpresentasikan oleh package model yang berisi class Hewan, Burung, dan Ikan. Bagian ini bertugas menyimpan data dan menyediakan constructor, atribut, serta method getter, setter, dan tampilkanInfo(). Controller direpresentasikan oleh package service melalui class HewanService, yang berfungsi mengatur logika program seperti operasi CRUD dan pencarian data. Sementara itu, View berada pada package main dengan class Main, yang menampilkan menu interaktif di console serta menerima input dari pengguna.








## Validasi Input







<img width="232" height="189" alt="image" src="https://github.com/user-attachments/assets/dc8d3789-e374-4554-9045-8f09616958a9" />








<img width="293" height="230" alt="image" src="https://github.com/user-attachments/assets/e5c0e5d1-138d-40b9-b861-3fb22c21d605" />







Program Klinik Hewan sudah dilengkapi dengan validasi input untuk memastikan data yang dimasukkan pengguna sesuai aturan. Pada saat menambahkan data hewan, input nomor HP pemilik tidak boleh kosong; jika kosong, program akan menampilkan pesan "No HP tidak boleh kosong!" dan proses penambahan data dibatalkan. Selain itu, input umur hewan harus lebih dari nol; jika pengguna memasukkan angka nol atau negatif, program akan menampilkan pesan "Umur hewan harus lebih dari 0!" dan data tidak akan disimpan.







## Fitur Search






<img width="411" height="273" alt="image" src="https://github.com/user-attachments/assets/6e3d8b27-fa15-424b-bd9c-fa22b71f1c2e" />







Program Klinik Hewan menyediakan fitur pencarian data hewan (search) untuk memudahkan pengguna menemukan informasi tertentu. Fitur ini bekerja dengan meminta pengguna memasukkan kata kunci berupa nama hewan, kemudian program akan melakukan pencocokan dengan seluruh data yang tersimpan di dalam ArrayList<Hewan>.






### encapsulation (getter dan setter)






<img width="677" height="354" alt="image" src="https://github.com/user-attachments/assets/6f097e13-dd8d-4657-9531-aa12d938f020" />








Program Klinik Hewan menerapkan konsep encapsulation dengan cara menjadikan semua atribut di dalam class Hewan, Burung, dan Ikan sebagai private, sehingga atribut-atribut tersebut tidak bisa diakses langsung dari luar class. Untuk mengakses dan mengubah nilai atribut, disediakan getter dan setter yang bersifat public.






### inheritance







<img width="296" height="236" alt="image" src="https://github.com/user-attachments/assets/70e1fae3-10bf-43ed-a23d-e7609c6b6658" />








<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/db80783c-0d9a-4e43-be6e-4a5c00938ecb" />








<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/94def4bb-e730-4db3-b217-68fedcce153e" />







<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/22f87f64-0416-4d66-abf9-7d19e2f7c31b" />







disini kita  menerapkan konsep inheritance (pewarisan) dengan menjadikan class Hewan sebagai superclass dan class Burung serta Ikan sebagai subclass. Class Hewan menyimpan atribut umum seperti namaPemilik, noHP, namaHewan, jenisHewan, umurHewan, dan keluhan. Class Burung mewarisi seluruh atribut dan method dari Hewan, lalu menambahkan atribut baru yaitu warnaBulu. Begitu juga dengan class Ikan yang mewarisi data dari Hewan serta menambahkan atribut khusus jenisAir.








### Overriding






<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/6a4d6a8b-e533-442d-924e-32657eb285ad" />









<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/d19dd47a-1a9d-41bf-aa50-84a740b77314" />









<img width="685" height="144" alt="image" src="https://github.com/user-attachments/assets/66d7be5e-16ae-4a46-9fc1-f04e6ff79f21" />








<img width="373" height="242" alt="image" src="https://github.com/user-attachments/assets/142079ea-b9ad-404a-8d79-f39c5ab56200" />










disini kita menerapkan konsep overriding, yaitu ketika subclass menuliskan ulang method yang sudah ada di superclass agar memiliki perilaku yang berbeda atau lebih spesifik. Pada class Hewan, terdapat method tampilkanInfo() yang menampilkan informasi umum hewan seperti nama pemilik, nomor HP, jenis hewan, umur, dan keluhan. Method ini kemudian dioverride di dalam subclass Burung dan Ikan. Pada class Burung, method tampilkanInfo() ditambahkan dengan informasi warna bulu serta pesan khusus mengenai perawatan burung. Sedangkan pada class Ikan, method yang sama ditambahkan dengan informasi jenis air serta perawatan khusus untuk ikan. Dengan overriding ini, meskipun method yang dipanggil sama (tampilkanInfo()), hasil output akan berbeda tergantung objeknya (Burung atau Ikan).











# Alur Program







<img width="186" height="122" alt="image" src="https://github.com/user-attachments/assets/de269e00-bbb2-4cd4-ab58-6f36e5e14f9c" />






Program memiliki 6 pilihan menu:





1. menu pertama yaitu tambah data, pada bagian ini user bakal diminta untuk mengisi data data seperti nama pemilik,nomor hp pemilik,nama hewan,jenis hewan,umur hewan, dan keluhan. pada pilihan jenis hewan kita disuruh pilih antara ikan, burung atau kita menuliskan hewan semau kita, kemudian pada no hp pemilik tidak boleh kosong, dan umur hewan tidak boleh kurang dari 0







<img width="304" height="294" alt="image" src="https://github.com/user-attachments/assets/f2e373c8-b62f-4ece-898e-ace322f14569" />








<img width="272" height="289" alt="image" src="https://github.com/user-attachments/assets/bc863dae-ebc4-43e7-a039-92f53c18fe79" />









<img width="299" height="279" alt="image" src="https://github.com/user-attachments/assets/8e773889-70dc-49fe-9f95-15b1e4f6c5df" />






dan ini adalh tampilan jika nomor hp kosng dan umur kurang dari 0 maka akan terkeluar sdari menambah data











<img width="231" height="203" alt="image" src="https://github.com/user-attachments/assets/2413b303-ac61-45a4-821c-a1a6a135de70" />








<img width="298" height="240" alt="image" src="https://github.com/user-attachments/assets/2af46780-360a-4b17-8c69-ee475a708e89" />









2. menu yang kedua adalah lihat data, dimenu ini program bakal menampilkan semua data yang sudah di tambahkan.








<img width="579" height="504" alt="image" src="https://github.com/user-attachments/assets/ab5ee127-59e6-416e-8c1c-254f0f1f9f95" />









dan ini adalah tampilan menu ke 2 jika data belum ada








<img width="255" height="195" alt="image" src="https://github.com/user-attachments/assets/15f4ab68-4590-4e0c-97ae-5dd628dd24ca" />










3.menu yang ketiga adalah ubah data, jadi pada menu ini user memilih nomor mana yang akan diubah, kemudian user mengubah datanya








<img width="422" height="536" alt="image" src="https://github.com/user-attachments/assets/23a8f519-6f99-4bda-8009-e7190a9c5acb" />









tampilan menu ke 3 jika nomor yang diinput tidak ada di data








<img width="438" height="526" alt="image" src="https://github.com/user-attachments/assets/16c38e33-003d-4111-a729-ae2d2e7c0ab4" />









4. menu yang keempat adalah hapus data, jadi dimenu ini user dapat menghapus data dengan memilih nomor yang ingin dihapus.







<img width="374" height="532" alt="image" src="https://github.com/user-attachments/assets/94e774b5-b4ff-4f99-9787-829763fb3cf1" />







tampilan menu ke 4 jika data yang mau di hapus tidak ada dalam data








<img width="399" height="431" alt="image" src="https://github.com/user-attachments/assets/46153d87-fe59-43fb-be45-bdcfc7c83d27" />








tampilan menu ke 4 jika data belum ada






<img width="206" height="192" alt="image" src="https://github.com/user-attachments/assets/5e24264c-3635-4f53-9b1b-daa8bfcfefd8" />











5. menu yang kelima adalah cari data hewan jadi disini user bisa mencari data hewan dengan menuliskan nama hewannya







<img width="440" height="265" alt="image" src="https://github.com/user-attachments/assets/5cce6ced-3906-424b-bab4-206e68e3c55c" />










6. menu ke enam adalah keluar,  jika user memilih menu ini maka program yang dijalankan akan selesai.







<img width="532" height="251" alt="image" src="https://github.com/user-attachments/assets/32a549a9-496d-43fb-a445-f00df0067d23" />








jika user memilih angka 7 atau seterusnya maka pilihan tidak valid








<img width="205" height="167" alt="image" src="https://github.com/user-attachments/assets/e9c88c7a-2575-4e3b-b53f-a67f0813b4c1" />









Program hanya akan berhenti jika user memilih menu Keluar (pilihan nomor 6).








