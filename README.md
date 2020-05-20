---
title: Dokumentasi WebApp Digitcard
author: Rian AP, Refianto DD, Yasmin RF
date: 2020
---

# Digitcard Documentation
## Nama Sistem
Digitcard

## Deskripsi Singkat
Digitcard adalah sebuah aplikasi berbasis web yang dapat mengakses dan menampilkan profil siswa dengan kode NIS yang sesuai.

## Ruang Lingkup Pengembangan
1. Digitcard dikembangkan untuk skala SMP Cendekia Baznas, dengan fungsi utama menampilkan profil murid beserta prestasi dan pelanggaran yang telah dilakukannya.
2. Digitcard hanya bisa diakses oleh guru, satpam, dan tenaga kependidikan lain karena hal ini menyangkut data pribadi siswa-siswi dari SMP Cendekia Baznas.

## Diagram
### Use Case Diagram
<p align="center"><img src="https://github.com/rdamaid/backend-scb-cec/raw/master/resources/useCaseDiagram.png" width="50%"></p>

### Activity Diagram
<p align="center"><img src="https://github.com/rdamaid/backend-scb-cec/raw/master/resources/activityDiagram.png" width="100%"></p>

### Class Diagram
<p align="center"><img src="https://github.com/rdamaid/backend-scb-cec/raw/master/resources/classDiagram.png" width="50%"></p>

## Fitur Secara Umum
1. Menggunakan multi-user dengan privilege masing-masing
2. Menampilkan capaian siswa

## Konsep OOP yang Digunakan
### Class
Menggunakan konsep Class
```
class User extends Authenticatable
{
   // Isi class User
}
```

### Inheritance
Menurunkan class User dari class Authenticatable
```
class User extends Authenticatable
{
   // Isi class User
}
```

### Enkapsulasi
Meskipun memiliki method yang sama, CRUD pada setiap class akan menghasilkan fungsi yang berbeda
```
class ProdukController extends Controller
{
    public function index() {}

    public function create() {}

    public function store(Request $request) {}
    
    public function show(Produk $produk) {}
    
    public function edit(Produk $produk) {}
    
    public function update(Request $request, Produk $produk) {}
    
    public function destroy(Produk $produk) {}

}
```


## Tipe Desain Pengembangan yang Digunakan
#### Anti-Pattern: Spaghetti Code
Memecah file Controller menjadi beberapa file untuk menghindari spaghetti code

#### Structural Design Pattern: Facade
Menggunakan facade untuk memudahkan penggunaan kembali kode yang sering digunakan
```
use Illuminate\Support\Facades\Auth;
```

## Developer
| Nama                     | Job Description              |
| ------------------------ | ---------------------------- |
| Rian Ardiana Prapanca    | Project Manager, Full Stack  |
| Refianto Damai Darmawan  | Back End Developer           |
| Yasmin Rizki Fairuza     | Front End Developer          |
