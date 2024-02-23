# project-kasir
## Background Problem
Andi adalah seorang pemilik supermarket besar di salah satu Indonesia. Andi memiliki rencana untuk melakukan perbaikan proses bisnis, yaitu Andi akan membuat sistem kasir yang self-service di supermarket miliknya. Sehingga customer bisa langsung memasukkan item yang dibeli, jumlah item yang dibeli, dan harga item yang dibeli dan fitur yang lain.
Sehingga customer yang tidak berada di kota tersebut bisa membeli barang dari supermarket tersebut. Setelah Andi melakukan riset, ternyata Andi memiliki masalah, yaitu Andi membutuhkan Programmer untuk membuatkan fitur-fitur agar bisa sistem kasir self-service di supermarket itu bisa berjalan dengan lancar.

---

## Requirements :
1. Customer memasukkan nama item, jumlah item, harga per item yang 
   ingin dibeli
2. Jika customer sudah selesai dengan berbelanjanya, tetapi masih apakah nama barang, jumlah barang, dan harga barang yang diinput sudah benar. Maka customer bisa melakukan check order. Menggunakan method check_order() dengan ketentuan :
    a). Jika transaksi sudah sesuai maka terdapat pesan “Pemesanan 
        Sudah Benar” lalu keluar output transaksi
    b). Jika terdapat kesalahan input maka akan mengeluarkan pesan 
        “terdapat kesalahan input data” dan bisa melakukan update item
   
3. Jika terjadi kesalahan pada saat customer memasukkan nama item,   
   jumlah item, atau harga per item tetapi tidak ingin menghapus 
   itemnya, maka customer dapat melakukan update :
   a). Update nama item dengan method :
       update_item_name
   b). Update jumlah item dengan method :
       update_item_jumlah
   c). Update harga per item dengan method :
       update_item_harga
   
4.  Jika customer ingin membatalkan transaksi maka bisa melakukan :
   a). Menghapus salah satu item dari nama item dengan method
       delete_item(<nama item>)
   
   b). reset all transactions
   
6. If the customers have finished purchasing, but are still unsure whether the price of the items and name entered are correct, the customers can check the order with the following output:
   
   a). Issue the message "Order is correct" if there are no input errors.
   
   b). Issue the message "There is a data input error" if an input error occurs.
   
   c). Displays a table containing all order data.
   
7. Finally, the customers can display the total price of the items which should be paid and the discount obtained (if any).
