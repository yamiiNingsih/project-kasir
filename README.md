# project-kasir
## Background Problem
Andi adalah seorang pemilik supermarket besar di salah satu Indonesia. Andi memiliki rencana untuk melakukan perbaikan proses bisnis, yaitu Andi akan membuat sistem kasir yang self-service di supermarket miliknya. Sehingga customer bisa langsung memasukkan item yang dibeli, jumlah item yang dibeli, dan harga item yang dibeli dan fitur yang lain.
Sehingga customer yang tidak berada di kota tersebut bisa membeli barang dari supermarket tersebut. Setelah Andi melakukan riset, ternyata Andi memiliki masalah, yaitu Andi membutuhkan Programmer untuk membuatkan fitur-fitur agar bisa sistem kasir self-service di supermarket itu bisa berjalan dengan lancar.

---

## Requirements :
* Customer memasukkan nama item, jumlah item, harga per item yang 
   ingin dibeli
* Jika customer sudah selesai dengan berbelanjanya, tetapi masih apakah nama barang, jumlah barang, dan harga barang yang diinput sudah benar. Maka customer bisa melakukan check order. Menggunakan method check_order() dengan ketentuan :
    * Jika transaksi sudah sesuai maka terdapat pesan “Pemesanan 
        Sudah Benar” lalu keluar output transaksi
    * Jika terdapat kesalahan input maka akan mengeluarkan pesan 
        “terdapat kesalahan input data” dan bisa melakukan update item
   
* Jika terjadi kesalahan pada saat customer memasukkan nama item,   
   jumlah item, atau harga per item tetapi tidak ingin menghapus 
   itemnya, maka customer dapat melakukan update :
   * Update nama item dengan method :
       update_item_name
   * Update jumlah item dengan method :
       update_item_jumlah
   * Update harga per item dengan method :
       update_item_harga
   
* Jika customer ingin membatalkan transaksi maka bisa melakukan :
   * Menghapus salah satu item dari nama item dengan method
       delete_item(<nama item>)
   * Jika ingin menghapus semua transaksi maka dapat menggunakan 
       method
      reset_transaction()
* Setelah selesai melakukan pengecekan,customer dapat menghitung total belanja yang sudah dibeli. Dengan menggunakan method total_harga(). Pada supermarket ini terdapat 
  ketentuan :
   * Jika total belanja customer diatas Rp 200.000 maka akan 
       mendapatkan diskon 5%
   * Jika total belanja customer diatas Rp 300.000 maka akan 
       mendapatkan diskon 8%
   * Jika total belanja customer diatas Rp 500.000 maka akan 
       mendapatkan diskon 10%
   
## Objectif :
Proyek ini bertujuan untuk membuat sistem kasir supermarket dengan alur sebagai berikut:
   * Pelanggan memasukkan nama barang, jumlah barang, dan harga 
       barang yang dibeli.
   * Jika terjadi kesalahan dalam memasukkan nama barang, jumlah 
       barang, atau harga barang, pelanggan dapat mengubah atau 
       memperbarui barang tersebut:
        * perbarui nama item
        * perbarui jumlah item
        * perbarui harga barang
   * Jika pelanggan membatalkan pembelian suatu barang, pelanggan 
       dapat menghapus barang tersebut:
        * hapus satu baris 
        * reset semua transaksi
   * Jika pelanggan sudah selesai membeli, namun masih ragu apakah 
       harga barang dan nama     yang dimasukkan sudah benar, 
       pelanggan dapat memeriksa pesanan dengan output sebagai 
       berikut:
        * Keluarkan pesan “Pesanan sudah benar” jika tidak ada 
          kesalahan input.
        * Mengeluarkan pesan “Ada kesalahan input data” jika terjadi 
          kesalahan input.
        * Menampilkan tabel yang berisi semua data pesanan.
    
## Flowchart
![image](https://github.com/yamiiNingsih/project-kasir/blob/main/Supermarket%20Andi-flowchart%20Supermarket.png)

## Function atau atribut yang dibuat
![image](https://github.com/yamiiNingsih/project-kasir/blob/main/method%20dan%20fungsi.jpeg)

## Test Case 1
add item dan check 

**Input:**<br />
1. `trnsct_123 = Transaction()'
2. 'trnsct_123.add_item("Ayam Goreng", 2, 20000)'
3. 'trnsct_123.add_item("Pasta Gigi", 3, 15000)'
4. 'trnsct_123.check_items()'

**Output:**<br />

![image](https://github.com/yamiiNingsih/project-kasir/blob/main/testing%201.jpeg)

## Test Case 2
delete item

**Input:**<br />
1. `trnsct_123.delete_item("Pasta Gigi")'
2. 'trnsct_123.check_items()'

**Output:**<br />

![image](https://github.com/yamiiNingsih/project-kasir/blob/main/testing%202.jpeg)

## Test Case 3
reset item

**Input:**<br />
1. 'trnsct_123.reset_transaction()'
2. 'trnsct_123.check_items()'

**Output:**<br />

![image](https://github.com/yamiiNingsih/project-kasir/blob/main/testing%203.jpeg)

## Test Case 4
check order

**Input:**<br />
1. 'trnsct_123 = Transaction()'
2. 'trnsct_123.add_item("Ayam Goreng", 2, 20000)'
3. 'trnsct_123.add_item("Pasta Gigi", 3, 15000)'
4. 'trnsct_123.add_item("Mainan Mobil", 1, 200000)'
5. 'trnsct_123.add_item("Mi Instan", 5, 3000)'
6. 'trnsct_123.check_order()''


**Output:**<br />

![image](https://github.com/yamiiNingsih/project-kasir/blob/main/testing%204.jpeg)

## Test case5
Menghitung Total yang harus dibayar

**Input:**<br />
1. 'trnsct_123.total_price()'
2. 'trnsct_123.check_items()''

![image](https://github.com/yamiiNingsih/project-kasir/blob/main/testing%205.jpeg)

## Kesimpulan
Sistem kasir swalayan dibuat dengan menggunakan bahasa pemrograman Python untuk memudahkan pelanggan dalam melakukan transaksi belanja. Sistem ini mempunyai beberapa fitur seperti menambah barang, memperbarui nama barang, memperbarui jumlah barang, memperbarui harga barang, menghapus satu barang, menghapus semua barang, menghitung total harga barang dan diskon yang diperoleh, serta menampilkan tabel belanja.

Karena sistem kasir ini berkonsep self-service, maka fitur-fiturnya masih dapat dikembangkan agar lebih ramah pengguna, seperti:

 * Menggunakan fitur input untuk membantu pelanggan menambah dan memperbarui/mengubah item yang ingin dibeli tanpa harus mengetikkan nama item secara manual.
 * Menyediakan katalog belanja atau daftar barang yang tersedia di supermarket yang terhubung dengan database untuk meminimalkan kesalahan.








 
 


