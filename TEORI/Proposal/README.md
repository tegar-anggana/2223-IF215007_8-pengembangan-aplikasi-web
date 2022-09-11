# :page_with_curl: Proposal: Aplikasi Web To-Do List & Jadwal untuk Mahasiswa IF UIN Sunan Gunung Djati
Proposal ini dibuat untuk memenuhi tugas [teori class CLO-0212 Project: Proposal](https://github.com/insanalamin/2223-IF215007_8-pengembangan-aplikasi-web#theory-class-2-credit) 

## :clipboard: Informasi Penulis

 - Nama : Tegar Levta Anggana
 - NIM : 1207050123
 - Jurusan/Kelas : Teknik Informatika/F
 
## :closed_book: Permasalahan
 - Mahasiswa memiliki banyak tugas dan jadwal yang berantakan
 - Mahasiswa kesulitan menemukan tugas / jadwal dengan kriteria tertentu yang berada di antara banyaknya tugas dan jadwal yang menumpuk
 
## :green_book: Rancangan Solusi
 - Aplikasi to-do list yang di dalamnya tugas-tugas / aktivitas bisa dicari, difilter, dan dikelompokkan.

## :ballot_box_with_check: Use Case
 - User bisa mengelola halaman, yang mana halaman terdiri atas tugas-tugas atau jadwal tertentu.
 - User bisa mengelola tugas-tugas yang ada.
 - User bisa mengelola properti-properti untuk tugas tertentu.
 - User bisa mencari dan mengelompokkan tugas.
 - User bisa memfilter tugas-tugas sesuai properti yang dimiliki tugas.

## :books: Struktur Data

### User
|Atribut|Tipe Data|Contoh|
|--|--|--|
|id|Integer|999|
|username|string|naruto|
|password|string|uzumaki|

### Halaman
|Atribut|Tipe Data|Contoh|
|--|--|--|
|id|Integer|999|
|judul|string|Tugas Kuliah|


### Aktivitas
|Atribut|Tipe Data|Contoh|
|--|--|--|
|id|Integer|999|
|judul|string|Membuat website e-commerce|

### Properti
|Atribut|Tipe Data|Contoh|
|--|--|--|
|id|Integer|999|
|nama|string|Mata Kuliah|
|nilai|string|Praktikum Pengembangan Aplikasi Web|

### Grup
|Atribut|Tipe Data|Contoh|
|--|--|--|
|id|Integer|999|
|nama|string|Favorit Ku|

## :house_with_garden: UX Wireframe 
<img width="656" alt="wireframe" src="https://user-images.githubusercontent.com/80917799/189483816-98d45cc7-8069-43cc-838b-5402fec84712.png">
<img width="542" alt="filter aktivitas" src="https://user-images.githubusercontent.com/80917799/189530005-f5587008-f523-4338-bf25-1e44a4ee2af1.png">
<img width="542" alt="jadwal kuliah" src="https://user-images.githubusercontent.com/80917799/189530009-29a865c9-3a0f-408c-a2f5-70137430d0fa.png">
<img width="542" alt="tambah aktivitas" src="https://user-images.githubusercontent.com/80917799/189530020-9fc5bb79-ca26-4b19-ae99-01f40ef8620f.png">
<img width="543" alt="tambah halaman" src="https://user-images.githubusercontent.com/80917799/189530023-ae4169a7-a5dd-4ccc-bfae-024f5c9658f7.png">

